<div align="center">

# ESPFlight Hardware Reference

**Open hardware reference design for ESP-based drones**

**Learn. Build. Modify. Create your own.**

[Website](https://espflight.com) · [Firmware](https://github.com/espflight/firmware) · Documentation

</div>

ESPFlight Hardware Reference provides an open and practical starting point for building and developing ESP-based drone hardware.

It is designed for enthusiasts, students, educators, Makers, developers, and engineers who want to study a working design, build it, modify it, experiment with different configurations, or use it as the foundation for their own hardware.

ESPFlight is an open platform, not a commercial drone kit brand. Hardware published by ESPFlight is provided as a reference design rather than as a required official product.

## About the Hardware Reference

The ESPFlight Hardware Reference demonstrates one practical implementation of hardware compatible with the ESPFlight platform.

It is a starting point, not a restriction on how ESPFlight-compatible hardware must be designed.

You can:

* Study the schematic and PCB design
* Build the reference hardware
* Modify the PCB layout
* Change the board shape or dimensions
* Adapt the design for different frames
* Use different compatible components
* Develop your own ESPFlight-compatible boards
* Create educational kits and independent products
* Use the design as a foundation for further experimentation and development

Hardware derived from ESPFlight may use its own independent name and branding.

## ESPFlight Platform

ESPFlight brings together:

* **Firmware** — open-source flight-control firmware
* **Hardware Reference** — open hardware designs
* **ESPFlight Application** — configuration and control application
* **Documentation** — build, setup, validation, and usage guides

Firmware:

https://github.com/espflight/firmware

Website:

https://espflight.com

## EasyEDA Project

The editable Hardware Reference is maintained in EasyEDA.

**EasyEDA project:**

`ADD_EASYEDA_PROJECT_LINK_HERE`

The EasyEDA project should be considered the primary editable source for the hardware design.

You can copy the project into your own EasyEDA workspace, inspect it, modify it, and develop your own compatible hardware implementation.

## Repository Structure

The repository may contain resources such as:

```text
hardware/
├── README.md
├── LICENSE
├── NOTICE.md
├── design/
│   └── EasyEDA project files and exports
├── schematic/
│   └── schematic exports
├── gerber/
│   └── PCB fabrication files
├── bom/
│   └── bill of materials
└── images/
    └── board and reference images
```

The exact files may vary between hardware revisions.

## Building the Reference Hardware

A typical workflow is:

1. Open the Hardware Reference in EasyEDA.
2. Review the schematic and PCB layout.
3. Copy the project into your own EasyEDA workspace if you want to modify it.
4. Review the BOM and component availability.
5. Verify the PCB revision and fabrication files.
6. Order the PCB and required components.
7. Assemble the hardware.
8. Inspect the completed board before applying power.
9. Flash compatible ESPFlight Firmware.
10. Perform hardware and firmware validation without propellers.
11. Verify motors, IMU orientation, control directions, ARM / DISARM, and failsafe behavior.
12. Proceed to controlled flight testing only after successful validation.

Always use the documentation that matches your hardware and firmware revision.

## Compatibility

A custom board does not need to look identical to the ESPFlight Hardware Reference to work with ESPFlight.

Compatibility depends on factors such as:

* ESP microcontroller or module
* Sensor support
* Electrical connections
* Motor outputs
* Pin assignments
* Power architecture
* Firmware configuration
* Communication requirements

Hardware changes may require corresponding firmware configuration or code changes.

The Hardware Reference should therefore be treated as a known working foundation that can be adapted and extended.

## Independent Hardware and Products

ESPFlight is designed to support independent hardware development.

Makers, developers, engineers, educators, teams, and other builders may create their own boards, kits, educational platforms, and products based on the Hardware Reference, subject to the applicable license.

Independent products should use their own product names and branding.

Using ESPFlight Firmware or deriving a design from the Hardware Reference does not make an independent product an official ESPFlight product.

Accurate descriptions such as:

* **Based on ESPFlight**
* **Compatible with ESPFlight**
* **Uses ESPFlight Firmware**

may be used in accordance with the ESPFlight Brand Policy.

## Fabrication Files

The repository may include fabrication resources such as Gerber files, schematic exports, and a BOM for convenience.

Before ordering a PCB:

* Confirm the hardware revision
* Review board dimensions
* Verify the PCB layer configuration
* Check footprints and component values
* Confirm component availability
* Review the fabrication requirements of your PCB service
* Verify that the Gerber files match the intended revision

If you modify the design, generate and verify your own fabrication files before ordering.

## Safety

Drone hardware can cause injury or property damage if assembled, configured, or operated incorrectly.

Before applying power or attempting flight:

* Inspect solder joints and assembly
* Check for electrical shorts
* Verify supply voltage and polarity
* Verify motor connections
* Verify motor direction
* Verify propeller direction
* Verify IMU orientation
* Verify control directions
* Verify ARM / DISARM behavior
* Verify communication failsafe behavior
* Perform initial testing without propellers where appropriate
* Keep people, animals, and property clear during testing

You are responsible for validating hardware that you build, modify, or operate.

Follow applicable safety requirements and local regulations.

## Contributions

Technical feedback and improvements are welcome.

Useful contributions may include:

* Schematic corrections
* PCB layout improvements
* Component substitutions
* BOM updates
* Fabrication notes
* Assembly documentation
* Validation results
* Tested hardware variants

Substantially different hardware designs should be clearly identified as independent ESPFlight-compatible implementations.

## Reporting Hardware Issues

When reporting a hardware-related issue, include relevant information whenever possible:

* Hardware revision
* ESP module or microcontroller
* Sensor configuration
* Power source
* Motor configuration
* Firmware version
* Description of the issue
* Steps to reproduce
* Measurements or images when useful

Clear technical information makes hardware issues significantly easier to investigate.

## License

The ESPFlight Hardware Reference is open hardware licensed under the **CERN Open Hardware Licence Version 2 — Permissive (CERN-OHL-P-2.0)**.

You may study, modify, build, distribute, and develop independent projects and products based on the Hardware Reference subject to the terms of the license.

The ESPFlight name, logo, visual identity, and other brand assets are not included in the open hardware license.

See [`LICENSE`](LICENSE) for the complete hardware license terms and [`NOTICE.md`](NOTICE.md) for additional information.

## Philosophy

ESPFlight provides a foundation that can be understood, modified, extended, and turned into something new.

**Learn it. Build it. Change it. Create your own.**

---

<div align="center">

**ESPFlight Hardware Reference**

https://espflight.com

</div>
