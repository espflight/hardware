# ESPFlight Hardware Reference v1.0 — Pinout

This document records the default firmware-facing pin mapping used by ESPFlight Firmware v1.0.0 with the ESPFlight Hardware Reference v1.0.

The authoritative firmware definitions are in the Firmware repository's `config.h`. Custom boards may use different mappings only when the corresponding firmware configuration and electrical design are changed and validated together.

## ESP8266 / Wemos D1 mini mapping

| Function | Wemos label | ESP8266 GPIO | ESPFlight v1.0 role |
| --- | --- | ---: | --- |
| Motor 1 | D1 | GPIO5 | Front-right motor |
| Motor 2 | D2 | GPIO4 | Rear-right motor |
| Motor 3 | D7 | GPIO13 | Rear-left motor |
| Motor 4 | D8 | GPIO15 | Front-left motor |
| Status LED | D4 | GPIO2 | ESPFlight status indication |
| Buzzer | RX | GPIO3 | Startup and failsafe buzzer |
| I2C SDA | D6 | GPIO12 | MPU6050 / shared sensor bus data |
| I2C SCL | D5 | GPIO14 | MPU6050 / shared sensor bus clock |

## I2C bus

ESPFlight v1.0.0 uses the shared I2C bus at 400 kHz.

- MPU6050 is mandatory for the v1.0 flight-control baseline and is addressed at `0x68`.
- VL53L0X is optional and is used by altitude-assisted functionality when detected and healthy.
- The reference firmware starts I2C with SDA on D6 / GPIO12 and SCL on D5 / GPIO14.

## Motor order

The default mixer and hardware mapping use this order:

```text
Motor 1 — Front Right
Motor 2 — Rear Right
Motor 3 — Rear Left
Motor 4 — Front Left
```

Do not change motor order, pin assignments, propeller direction, or mixer assumptions independently. Any such change must be treated as a hardware/firmware configuration change and validated without propellers before powered flight.

## ESP8266 pin cautions

- GPIO15 / D8 is an ESP8266 boot-strap pin. The v1.0 reference design and firmware mapping were validated around the published hardware implementation; custom hardware must preserve valid boot conditions.
- GPIO3 / RX is the ESP8266 UART receive pin. ESPFlight v1.0 intentionally assigns it to the buzzer path in the reference configuration.
- GPIO2 / D4 also participates in ESP8266 boot behavior. Custom external circuitry must not force an invalid boot state.

## Power and off-board connections

This file documents firmware-facing signal pins. It does not replace the schematic, assembly notes, power-path review, or polarity checks.

Before power-up:

1. Review the public EasyEDA schematic and PCB.
2. Read `docs/ASSEMBLY_NOTES.md`.
3. Verify supply voltage and polarity.
4. Check for shorts.
5. Validate motor and sensor connections.
6. Perform initial firmware tests without propellers.

## Version scope

This mapping applies to:

- ESPFlight Firmware v1.0.0
- ESPFlight Hardware Reference v1.0
- ESPFlight Protocol 2

Independent or later hardware revisions must publish their own explicit mapping when it differs from this baseline.
