# Editable Hardware Source

This directory contains versioned editable hardware-design snapshots.

## ESPFlight Hardware Reference v1.0

The current `main` branch includes the editable EasyEDA project export:

**[ESPFlight_Hardware_Reference_v1.0_EasyEDA_Source.zip](ESPFlight_Hardware_Reference_v1.0_EasyEDA_Source.zip)**

The archive contains the EasyEDA source for both the schematic and PCB, together with the project README exported from the official v1.0 EasyEDA project.

The public online project remains available at:

https://oshwlab.com/eng_karimizadeh/project_xfbshxkb

### Integrity

SHA-256:

```text
876164299499c7eddd6da02b3eaf02faebfa2f2027e284bb83c3caee09396821
```

Git blob SHA:

```text
b3708b0960879348ee7bdf14bb1cc9d795362e14
```

The Git blob SHA above matches the uploaded ZIP stored in this repository.

## Release provenance

The published `v1.0` tag predates this GitHub-hosted editable-source snapshot and remains immutable.

The validated Gerber, BOM, and Pick-and-Place files in the official v1.0 release remain the authoritative fabrication baseline for that published release. The editable EasyEDA snapshot was added later to the current `main` branch to preserve the original project source without rewriting the existing release tag.

Future Hardware Reference releases must include the corresponding editable source snapshot as part of the release baseline before publication.

Do not reconstruct or approximate editable source from Gerber files and present it as the original source.

See [`../RELEASE_POLICY.md`](../RELEASE_POLICY.md) for release requirements.
