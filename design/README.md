# Editable Hardware Source

This directory is reserved for versioned editable hardware-design snapshots.

## ESPFlight Hardware Reference v1.0

The original public v1.0 GitHub package contains the validated fabrication outputs, BOM, Pick-and-Place data, assembly notes, checksums, and licensing material, but it does **not** contain a native editable EasyEDA project export.

The current public editable source for v1.0 remains the official EasyEDA project:

https://oshwlab.com/eng_karimizadeh/project_xfbshxkb

The v1.0 tag must remain immutable, so an editable export must not be retroactively inserted into that published tag.

## Future baselines

Before the next Hardware Reference baseline is released, place the corresponding native/editable EasyEDA export in this directory and verify that it represents the same design revision used to generate the release fabrication files.

Do not reconstruct or approximate an editable source from Gerber files and present it as the original source.

See ../RELEASE_POLICY.md for the release requirements.
