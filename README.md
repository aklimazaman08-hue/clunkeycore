## PCB Design

![ClunkeyCore PCB layout]

<img width="2360" height="1391" alt="image" src="https://github.com/user-attachments/assets/e0ce242b-215e-4682-bb2e-fe443181753b" />


# ClunkeyCore — ESP32 Robotics Controller

ClunkeyCore is a PCB control-board design for my Clunkey Rover, a four-wheel robotics project inspired by my experience with FIRST Robotics.

The board is designed around an ESP32-C5 and organizes the rover's motor connections, ultrasonic obstacle detection, power connections, and GPIO expansion.

## Features

- ESP32-C5 controller
- Four motor connections
- Two motor-driver placeholder footprints
- HC-SR04 ultrasonic sensor connection
- 2 kΩ / 3.3 kΩ voltage-divider network for the HC-SR04 ECHO signal
- 4×AA battery power input
- 8-pin GPIO expansion header
- PCB layout and routing designed in Protoboard Designer

## Motor Connections

The board provides four motor outputs:

- Motor 1 → TB6612 #2 placeholder
- Motor 2 → TB6612 #2 placeholder
- Motor 3 → TB6612 #1 placeholder
- Motor 4 → TB6612 #1 placeholder

The motor-driver footprints are placeholders because the exact TB6612 module footprint was not available in the design software.

## Ultrasonic Sensor

The HC-SR04 connections are:

- VCC → ESP32 5V
- TRIG → GPIO4
- ECHO → voltage divider → GPIO5
- GND → ESP32 GND

The voltage divider uses:

- R1 = 2 kΩ
- R2 = 3.3 kΩ

## GPIO Expansion

The 8-pin expansion header is connected to:

| Header Pin | ESP32 GPIO |
|------------|------------|
| 1 | GPIO6 |
| 2 | GPIO7 |
| 3 | GPIO8 |
| 4 | GPIO9 |
| 5 | GPIO10 |
| 6 | GPIO3 |
| 7 | GPIO2 |
| 8 | GPIO1 |

## Power

The PCB includes a power input intended for a 4×AA battery holder.

The current PCB is a design prototype. The final power regulation and exact component selection will need to be verified before connecting an actual battery or manufacturing the board.

## Design Status

This project is currently a PCB design/prototype.

The board has been routed and visually reviewed, but it has **not been physically manufactured or electrically tested**.

The motor-driver footprints are placeholders and should be replaced with a verified footprint and pinout for the exact TB6612 module before manufacturing.

## Inspiration

ClunkeyCore is part of my robotics work inspired by FIRST Robotics and my experience designing and working with competition robots.

The project is named after Clunkey, my team's robotics mascot.
