# ESPFlight Hardware Reference v1.0 — Release Notes

**Release:** v1.0  
**Release date:** 2026-09-01

ESPFlight Hardware Reference v1.0 is the first frozen public hardware-reference release for the ESPFlight platform.

## Included

- Final two-layer PCB fabrication Gerbers
- Final BOM
- Final Pick-and-Place data
- CERN-OHL-P-2.0 licensing notice
- Assembly notes
- SHA-256 checksums

## Final v1.0 validation changes

Before release, the fabrication package and metadata were reviewed for consistency. The final baseline includes:

- 0805 ferrite beads on the intended power branches (`L1`, `L2`)
- corrected 100 nF / 0805 capacitor selections
- corrected `R13` 1 kΩ / 0805 part selection
- synchronized diode designators `D1`–`D4`
- synchronized buzzer designator
- synchronized MOSFET designators `Q1`–`Q4`
- synchronized 10 kΩ resistor metadata for `R2`, `R4`, `R6`, and `R8`
- matching BOM and Pick-and-Place footprints for PCB-mounted BOM components

## Release status

**ESPFlight Hardware Reference v1.0 — FINAL**

This baseline should remain frozen. Future electrical or PCB changes should be released as a new hardware revision rather than silently replacing v1.0.
