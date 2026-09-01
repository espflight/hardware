<div align="center">

# ESPFlight Hardware Reference

**Open hardware reference design for ESP-based drones**

**Learn it. Build it. Change it. Create your own.**

[Website](https://espflight.com) · [Firmware](https://github.com/espflight/firmware) · [Documentation](https://espflight.com/docs/) · [Brand Policy](https://espflight.com/brand-policy/)

**Hardware Reference v1.0**

</div>

ESPFlight Hardware Reference provides an open and practical starting point for building and developing ESP-based drone hardware.

It is designed for enthusiasts, students, educators, Makers, developers, and engineers who want to study a working design, build it, modify it, experiment with different configurations, or use it as the foundation for their own hardware.

ESPFlight is an open platform, not a commercial drone-kit brand. Hardware published by ESPFlight is provided as a reference design rather than as a required official product.

## Release v1.0

This release contains the validated fabrication outputs for **ESPFlight Hardware Reference v1.0**:

- Gerber fabrication package
- Bill of Materials (BOM)
- Pick-and-Place file
- Assembly notes
- Release notes and checksums

The editable hardware source is maintained in EasyEDA. The current public project link is published through:

https://espflight.com/hardware/

## Fabrication Files

```text
fabrication/
├── gerber/
│   └── ESPFlight_Hardware_Reference_v1.0_Gerber.zip
├── bom/
│   └── ESPFlight_Hardware_Reference_v1.0_BOM.csv
└── pick-and-place/
    └── ESPFlight_Hardware_Reference_v1.0_PickAndPlace.csv
```

The Gerber archive includes two copper layers, solder mask, silkscreen, paste layers, board outline, document layer, plated-through-hole drill data, and via drill data.

## Manual / Module Components

Some parts are installed as modules or off-board/manual components and are therefore not included in the SMD BOM used for automated assembly.

These include the battery connection, MPU-6050 module, Wemos D1 mini module, and the associated through-hole/header connection used by the reference build.

See [`docs/ASSEMBLY_NOTES.md`](docs/ASSEMBLY_NOTES.md) before ordering assembly.

## Building the Reference Hardware

A typical workflow is:

1. Open the current ESPFlight Hardware Reference in EasyEDA.
2. Review the schematic and PCB revision.
3. Use the provided Gerber package for PCB fabrication, or generate fresh fabrication files from your own modified design.
4. Review the BOM and component availability.
5. Review the Pick-and-Place file if automated assembly will be used.
6. Assemble the remaining manual/module components.
7. Inspect the completed hardware before applying power.
8. Flash compatible ESPFlight Firmware.
9. Perform validation without propellers first.
10. Verify motor direction, IMU orientation, controls, ARM / DISARM, and failsafe behavior before controlled flight testing.

## Compatibility

A custom board does not need to look identical to the ESPFlight Hardware Reference to work with ESPFlight.

Compatibility depends on factors such as the ESP microcontroller or module, sensor support, electrical connections, motor outputs, pin assignments, power architecture, firmware configuration, and communication requirements.

Hardware changes may require corresponding firmware configuration or code changes.

## Independent Hardware and Products

ESPFlight is designed to support independent hardware development.

Builders may create their own boards, educational platforms, kits, and products based on the Hardware Reference, subject to the applicable license.

Independent products should use their own product names and branding. Using ESPFlight Firmware or deriving a design from the Hardware Reference does not make an independent product an official ESPFlight product.

Accurate factual descriptions such as **Based on ESPFlight**, **Compatible with ESPFlight**, and **Uses ESPFlight Firmware** may be used in accordance with the ESPFlight Brand Policy.

## Safety

Drone hardware can cause injury or property damage if assembled, configured, or operated incorrectly.

Before applying power or attempting flight:

- inspect solder joints and assembly;
- check for electrical shorts;
- verify supply voltage and polarity;
- verify motor and propeller direction;
- verify IMU orientation and control directions;
- verify ARM / DISARM behavior;
- verify communication failsafe behavior;
- perform initial testing without propellers where appropriate;
- keep people, animals, and property clear during testing.

You are responsible for validating hardware that you build, modify, or operate. Follow applicable safety requirements and local regulations.

## License

The ESPFlight Hardware Reference is licensed under the **CERN Open Hardware Licence Version 2 — Permissive (CERN-OHL-P-2.0)**.

See [`LICENSE`](LICENSE) and [`NOTICE.md`](NOTICE.md).

The definitive, unmodified CERN-OHL-P-2.0 text is published by CERN/Open Hardware Repository:

https://ohwr.org/cern_ohl_p_v2.txt

The ESPFlight name, logo, visual identity, and other brand assets are not included in the open-hardware license and remain subject to the ESPFlight Brand Policy.

## Philosophy

ESPFlight provides a foundation that can be understood, modified, extended, and turned into something new.

**Learn it. Build it. Change it. Create your own.**

---

<div align="center">

**ESPFlight Hardware Reference v1.0**

https://espflight.com

</div>
