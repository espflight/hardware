<div align="center">

# ESPFlight Hardware Reference

**Open hardware reference design for ESP-based drones**

**Learn it. Build it. Change it. Create your own.**

[Website](https://espflight.com) · [Build v1.0](https://github.com/espflight/docs/blob/main/BUILD_V1.0.md) · [Firmware](https://github.com/espflight/firmware) · [Documentation](https://espflight.com/docs/) · [Application](https://github.com/espflight/application) · [EasyEDA Project](https://oshwlab.com/eng_karimizadeh/project_xfbshxkb) · [Editable Source](design/ESPFlight_Hardware_Reference_v1.0_EasyEDA_Source.zip) · [Pinout](PINOUT.md) · [Release Policy](RELEASE_POLICY.md) · [Brand Policy](https://espflight.com/brand-policy/)

**Hardware Reference v1.0**

</div>

ESPFlight Hardware Reference provides an open and practical starting point for building and developing ESP-based drone hardware.

It is designed for enthusiasts, students, educators, Makers, developers, and engineers who want to study a working design, build it, modify it, experiment with different configurations, or use it as the foundation for their own hardware.

ESPFlight is an open platform, not a commercial drone-kit brand. Hardware published by ESPFlight is provided as a reference design rather than as a required official product.

## Start with ESPFlight v1.0

For the shortest official path from hardware to first controlled flight, see:

**[Build ESPFlight v1.0](https://github.com/espflight/docs/blob/main/BUILD_V1.0.md)**

## Release v1.0

The published v1.0 release contains the validated fabrication outputs for **ESPFlight Hardware Reference v1.0**:

- Gerber fabrication package
- Bill of Materials (BOM)
- Pick-and-Place file
- Assembly notes
- Release notes and checksums

The editable hardware design is available in two forms on the current project baseline:

- **[Download the EasyEDA source snapshot](design/ESPFlight_Hardware_Reference_v1.0_EasyEDA_Source.zip)**
- **[Open the public EasyEDA project](https://oshwlab.com/eng_karimizadeh/project_xfbshxkb)**

The official GitHub Release remains the immutable validated v1.0 fabrication baseline for Gerber, BOM, and Pick-and-Place files.

The original published v1.0 tag did not contain a native editable EasyEDA export. A source snapshot exported from the official v1.0 EasyEDA project was added later to the current `main` branch without modifying the published tag. Future hardware baselines must include the corresponding versioned editable design source as part of the release baseline, as defined in [RELEASE_POLICY.md](RELEASE_POLICY.md).

## Licensing source of truth

The versioned ESPFlight licensing statement for this hardware is defined by the `LICENSE` and `NOTICE.md` files in this GitHub repository.

The public OSHWLab project is provided as an online viewing/editing mirror and may display platform-generated reproduction or intellectual-property notices that are not project-specific. Those platform UI notices are not used as the ESPFlight release or licensing source of truth.

ESPFlight Hardware Reference is released under **CERN-OHL-P-2.0**. Commercial use, including independently branded boards, kits, and products, is permitted subject to the license terms and the separate ESPFlight Brand Policy.


## Fabrication Files

```text
fabrication/
├── gerber/
│   └── ESPFlight_Hardware_Reference_v1.0_Gerber.zip
├── bom/
│   └── ESPFlight_Hardware_Reference_v1.0_BOM.csv
└── pick-and-place/
    └── ESPFlight_Hardware_Reference_v1.0_PickAndPlace.csv

design/
├── ESPFlight_Hardware_Reference_v1.0_EasyEDA_Source.zip
└── README.md
```

The Gerber archive includes two copper layers, solder mask, silkscreen, paste layers, board outline, document layer, plated-through-hole drill data, and via drill data.

The editable source ZIP contains the EasyEDA project export for the schematic and PCB. See [`design/README.md`](design/README.md) for source provenance and integrity information.

## Pinout and firmware-facing interfaces

The default v1.0 firmware-facing pin mapping is documented in:

**[PINOUT.md](PINOUT.md)**

Custom boards may use different mappings only when the electrical design and corresponding firmware configuration are changed and validated together.

## Manual / Module Components

Some parts are installed as modules or off-board/manual components and are therefore not included in the SMD BOM used for automated assembly.

These include the battery connection, MPU-6050 module, Wemos D1 mini module, and the associated through-hole/header connection used by the reference build.

See [`docs/ASSEMBLY_NOTES.md`](docs/ASSEMBLY_NOTES.md) before ordering assembly.

## Building the Reference Hardware

A typical workflow is:

1. Open the [ESPFlight Hardware Reference v1.0 EasyEDA project](https://oshwlab.com/eng_karimizadeh/project_xfbshxkb) or download the [versioned EasyEDA source snapshot](design/ESPFlight_Hardware_Reference_v1.0_EasyEDA_Source.zip).
2. Review the schematic and PCB revision.
3. Review the [v1.0 pinout](PINOUT.md).
4. Use the provided Gerber package for PCB fabrication, or generate fresh fabrication files from your own modified design.
5. Review the BOM and component availability.
6. Review the Pick-and-Place file if automated assembly will be used.
7. Assemble the remaining manual/module components.
8. Inspect the completed hardware before applying power.
9. Flash compatible ESPFlight Firmware.
10. Perform validation without propellers first.
11. Verify motor direction, IMU orientation, controls, ARM / DISARM, and failsafe behavior before controlled flight testing.

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

The current `main` branch contains the complete unmodified CERN-OHL-P-2.0 text. The published v1.0 tag remains immutable; the packaging strategy for later baselines is documented in [RELEASE_POLICY.md](RELEASE_POLICY.md).

The ESPFlight name, logo, visual identity, and other brand assets are not included in the open-hardware license and remain subject to the ESPFlight Brand Policy.

## Philosophy

ESPFlight provides a foundation that can be understood, modified, extended, and turned into something new.

**Learn it. Build it. Change it. Create your own.**

---

<div align="center">

**ESPFlight Hardware Reference v1.0**

https://espflight.com

</div>
