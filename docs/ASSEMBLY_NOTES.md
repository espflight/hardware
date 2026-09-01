# ESPFlight Hardware Reference v1.0 — Assembly Notes

## Automated assembly files

The BOM and Pick-and-Place files in this release cover the PCB-mounted parts represented in the final v1.0 fabrication export.

Before submitting an automated PCBA order, verify current component availability and assembly-service rules.

## Manual / module components

The following items appear in the PCB placement data but are intentionally treated as module, connector, or off-board/manual-install items rather than ordinary SMD BOM parts:

- **BATTERY** — battery connection / off-board power source
- **MPU-6050** — MPU-6050 sensor module
- **U1** — through-hole/header connection used by the reference build
- **WEMOSD1MINI** — Wemos D1 mini module

These items should be sourced and installed according to the reference build and current documentation.

## Key v1.0 PCB parts

The final v1.0 release includes, among other components:

- `L1`, `L2` — Murata BLM21PG221SN1D ferrite beads, 0805, LCSC C85840
- `R13` — 1 kΩ, 0805, UNI-ROYAL 0805W8F1001T5E, LCSC C17513
- `D1`–`D4` — PMEG3020EGWX Schottky diodes
- `Q1`–`Q4` — FSS2302S / A2SHB-compatible MOSFET implementation used by this reference revision

## Before power-up

1. Check for shorts between supply and ground.
2. Verify battery polarity.
3. Verify module orientation and header alignment.
4. Inspect all solder joints.
5. Verify motor wiring and polarity.
6. Perform initial firmware validation without propellers.
