ESPFlight Hardware Reference

Open hardware reference design for ESPFlight-compatible drones.

ESPFlight Hardware Reference provides a practical starting point for makers, developers, students, and independent hardware builders who want to design and build small drones based on ESP microcontrollers and the ESPFlight platform.

ESPFlight is a platform, not a hardware manufacturer.
ESPFlight does not produce or sell an official ESPFlight-branded drone, flight controller, or hardware kit. This repository exists as an open reference that others can study, modify, manufacture, and build upon.

About the Hardware Reference

The ESPFlight Hardware Reference is intended to demonstrate one practical implementation of ESPFlight-compatible hardware.

It is not the only supported design.

Makers and companies are encouraged to:

Modify the PCB

Change the board shape or layout

Adapt the design for different frames

Use different compatible components

Create their own ESPFlight-compatible boards

Build educational kits or independent products based on the platform

The goal is to provide a reusable hardware foundation rather than create a closed hardware ecosystem.

ESPFlight Platform

ESPFlight consists of several independent parts:

Firmware — open-source flight controller firmware

Hardware Reference — open hardware design

ESPFlight Application — free control application

Documentation — build, setup, and usage guides

Firmware repository:

https://github.com/espflight/firmware

Website:

https://espflight.com

EasyEDA Project

The editable ESPFlight Hardware Reference is maintained in EasyEDA.

EasyEDA project:

ADD_EASYEDA_PROJECT_LINK_HERE

The EasyEDA project should be considered the primary editable hardware design source.

You can open the project, copy it to your own workspace, modify it, and create your own compatible hardware implementation.

Repository Structure

The repository may contain the following resources:

hardware/
├── README.md
├── LICENSE
├── design/
│   └── EasyEDA project files / exports
├── schematic/
│   └── schematic exports
├── gerber/
│   └── PCB manufacturing files
├── bom/
│   └── bill of materials
└── images/
    └── board and reference images

Not every folder is required for every hardware revision.

Building Your Own Hardware

A typical workflow is:

Open the reference design in EasyEDA.

Review the schematic and PCB layout.

Copy the project into your own EasyEDA workspace.

Modify the design if required.

Review the BOM and component availability.

Generate or use the provided Gerber files.

Order the PCB from a PCB manufacturer.

Assemble the components.

Inspect the board carefully before applying power.

Flash the ESPFlight firmware.

Test the system without propellers.

Verify motor direction, IMU orientation, controls, and failsafe behavior.

Proceed to controlled flight testing.

Always verify the latest documentation before building.

Compatibility

A custom board does not need to look identical to the reference PCB to be ESPFlight-compatible.

Compatibility depends on the electrical design, supported sensors, motor outputs, pin assignments, firmware configuration, and communication requirements.

If you change hardware connections or components, corresponding firmware configuration changes may also be required.

The Hardware Reference should therefore be treated as a known starting point, not as a restriction on future designs.

Independent Hardware and Products

Independent makers, teams, educators, and companies may create their own hardware based on ESPFlight.

Compatible products do not become official ESPFlight products simply because they use ESPFlight firmware or follow the Hardware Reference.

Third-party hardware should use its own product name and branding and clearly describe its relationship to ESPFlight.

This separation is intentional: ESPFlight is designed to remain an open platform that multiple independent hardware projects can build upon.

Safety

Drone hardware can cause injury or property damage if assembled, configured, or operated incorrectly.

Before powered flight:

Inspect all solder joints

Check for shorts

Verify supply voltage and polarity

Verify motor connections

Verify motor direction

Verify propeller direction

Verify IMU orientation

Verify control directions

Verify ARM / DISARM behavior

Verify communication failsafe

Test without propellers first

Keep people, animals, and property clear during testing

Use appropriate protective equipment and follow applicable local laws and regulations.

ESPFlight hardware designs are provided without warranty. You are responsible for validating any hardware you manufacture or operate.

Manufacturing

The Hardware Reference may include manufacturing files such as Gerbers and a BOM for convenience.

Before ordering boards:

Review the latest revision

Verify board dimensions

Verify layer configuration

Check component footprints

Confirm component availability

Review manufacturer design-rule requirements

If you modify the reference design, regenerate and verify your own manufacturing files.

Contributions

Hardware improvements and technical feedback are welcome.

Useful contributions may include:

Schematic corrections

PCB layout improvements

New compatible board designs

Component substitutions

BOM improvements

Manufacturing notes

Assembly documentation

Tested hardware variants

For substantial new hardware designs, consider clearly identifying the design as an independent ESPFlight-compatible implementation.

Reporting Hardware Issues

When reporting a hardware issue, include as much relevant information as possible:

Board revision

ESP module used

Sensor configuration

Power source

Motor / ESC configuration

Firmware version

Clear description of the problem

Steps to reproduce

Photos or measurements when useful

License

The hardware files in this repository are distributed under the license included in the repository.

See:

LICENSE

for the complete terms.

Different software components of the ESPFlight platform may use separate licenses. Always check the license included with each repository or component.

ESPFlight Philosophy

ESPFlight exists to make ESP-based flight experimentation easier to access, understand, modify, and extend.

The Hardware Reference is intentionally open-ended.

It provides a working foundation while leaving room for makers and independent companies to create different boards, frames, kits, educational platforms, and products around the same ecosystem.

Build it. Modify it. Learn from it. Make it your own.

ESPFlight

Open platform for building ESP-based drones.

https://espflight.com
