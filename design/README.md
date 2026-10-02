# Editable Hardware Source

This directory contains versioned editable hardware-design snapshots.

## ESPFlight Hardware Reference v1.0

The current `main` branch includes the editable EasyEDA project export:

**[ESPFlight_Hardware_Reference_v1.0_EasyEDA_Source.zip](ESPFlight_Hardware_Reference_v1.0_EasyEDA_Source.zip)**

The archive contains the EasyEDA source for both the schematic and PCB, together with the project README exported from the official v1.0 EasyEDA project.

The public online project remains available at:

https://oshwlab.com/eng_karimizadeh/project_xfbshxkb

For release provenance and project-specific licensing, this GitHub repository is authoritative. The OSHWLab page is an online viewing/editing mirror and may include platform-generated reproduction or intellectual-property notices. ESPFlight Hardware Reference remains licensed under CERN-OHL-P-2.0 as stated in the repository `LICENSE` and `NOTICE.md` files.


### Integrity

SHA-256:

```text
fc1595e9a2464167da13b810ad9e3be4733d2ce9372f3bd963535b6f2daee06d
```

Git blob SHA:

```text
2acc70177d810c5c6d73941623f96b7bee885439
```

The Git blob SHA above matches the uploaded ZIP stored in this repository.

### R13 metadata correction

On 2026-10-02, the GitHub-hosted editable EasyEDA snapshot received a metadata-only correction for `R13`.

The PCB geometry, routing, pads, vias, copper areas, schematic, and embedded project README were not changed. The correction updates the PCB component metadata to match the already-authoritative v1.0 BOM:

- value: `1 kΩ`;
- package: `R0805`;
- manufacturer part: `0805W8F1001T5E`;
- manufacturer: `UNI-ROYAL`;
- LCSC part: `C17513`;
- JLCPCB classification: `Basic Part`.

The validated Gerber, BOM, and Pick-and-Place files in the official `v1.0` release remain unchanged and authoritative.

## Release provenance

The published `v1.0` tag predates this GitHub-hosted editable-source snapshot and remains immutable.

The validated Gerber, BOM, and Pick-and-Place files in the official v1.0 release remain the authoritative fabrication baseline for that published release. The editable EasyEDA snapshot was added later to the current `main` branch to preserve the original project source without rewriting the existing release tag.

Future Hardware Reference releases must include the corresponding editable source snapshot as part of the release baseline before publication.

Do not reconstruct or approximate editable source from Gerber files and present it as the original source.

See [`../RELEASE_POLICY.md`](../RELEASE_POLICY.md) for release requirements.
