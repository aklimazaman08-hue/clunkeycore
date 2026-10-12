# ClunkeyCore — Bill of Materials

| Component | Quantity | Purpose | Status |
|---|---:|---|---|
| ESP32-C5 DevKitC-1 | 1 | Main microcontroller | Planned |
| HC-SR04 ultrasonic sensor | 1 | Obstacle detection | Planned |
| 2 kΩ resistor | 1 | ECHO voltage divider | Planned |
| 3.3 kΩ resistor | 1 | ECHO voltage divider | Planned |
| TB6612FNG motor driver module | 2 | Four-motor control | Placeholder footprint |
| 4×AA battery holder with switch | 1 | Battery power source | Planned |
| 4WD motor/chassis assembly | 1 | Rover drivetrain | Planned |
| 8-pin GPIO header | 1 | GPIO expansion | Designed |
| Motor connectors | 4 | Connect motors to the PCB | Designed |

## Notes

- The PCB was designed using Protoboard Designer.
- The two TB6612FNG footprints are visual placeholders because the exact module footprint was not available in the software.
- The exact TB6612FNG module pinout and footprint must be verified before manufacturing.
- The 4×AA battery holder is the planned power source.
- The PCB has not been physically manufactured or electrically tested.
- Component availability and final part selection may change before a physical build.
