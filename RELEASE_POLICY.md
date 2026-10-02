# ESPFlight Hardware Reference — Release Policy

This policy defines how future ESPFlight Hardware Reference baselines are packaged and versioned.

## Published v1.0 remains immutable

The existing `v1.0` tag and GitHub Release are historical release artifacts and must not be rewritten, force-moved, or replaced.

The current `main` branch contains repository-maintenance improvements made after the original publication, including the complete unmodified CERN-OHL-P-2.0 license text.

Release reproducibility takes priority over retroactively rewriting the published tag.

## License packaging for the next baseline

Every future Hardware Reference release must contain, inside the tagged source tree:

1. the complete, unmodified CERN Open Hardware Licence Version 2 — Permissive text in `LICENSE`;
2. the ESPFlight-specific notices in `NOTICE.md`;
3. clear identification of the covered hardware source;
4. the applicable ESPFlight Brand Policy reference;
5. third-party notices where required.

A release must not rely only on an external URL for the complete license text.

## Editable hardware source requirement

Before a new hardware baseline is published, the repository must include a versioned editable design snapshot corresponding to that release.

The preferred structure is:

```text
design/
├── README.md
└── <EasyEDA editable project export>

fabrication/
├── gerber/
├── bom/
└── pick-and-place/
```

The editable snapshot must correspond to the same design revision used to generate the release fabrication outputs.

The public EasyEDA / OSHWLab project may remain a convenient online viewing and editing mirror, but the GitHub repository, signed tag, and GitHub Release are the versioned source of truth for release provenance, licensing, and preserved release artifacts.

External platform-generated notices or UI text must not be relied on as the ESPFlight project-specific license statement. The tagged `LICENSE` and `NOTICE.md` files define the ESPFlight licensing statement for each published hardware baseline.

The GitHub tag must preserve a self-contained editable snapshot whenever the export format is available.

## Versioning

Use a patch release, such as `v1.0.1`, only when the electrical design and fabrication baseline remain unchanged and the release corrects packaging, documentation, metadata, or other non-electrical release material.

Use a new minor hardware revision, such as `v1.1`, when any PCB, schematic, footprint, component value, routing, connector, pin assignment, power path, or other hardware behavior changes.

Do not replace fabrication files under an existing published tag.

## Release integrity

For future official releases:

- release from a reviewed commit;
- require the applicable CI/checks to pass;
- use a verified signed release tag when the maintainer signing setup is available;
- publish SHA-256 checksums for fabrication archives and other release assets;
- keep published tags immutable;
- record compatibility with the corresponding Firmware, Application, and Protocol versions.

## v1.0 license correction strategy

No change will be made to the existing `v1.0` tag.

The complete CERN-OHL-P-2.0 text already present on `main` is the required packaging model for the next Hardware Reference release. If a dedicated packaging-only patch release is created before any electrical revision, it may be versioned as `v1.0.1` and must explicitly state that the hardware design and fabrication outputs are unchanged from v1.0.
