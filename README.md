# ESP32-S3 Custom Development Board

A custom ESP32-S3-MINI based development board designed for embedded system prototyping, USB-C powered development, onboard sensing, and hardware integration.

---

## Overview

This project focuses on the design of a compact custom ESP32-S3 development board with USB-C interface, regulated 3.3V power, onboard sensing, boot/reset circuitry, and GPIO breakout headers.

The board was designed to support reliable embedded prototyping and future hardware integration projects.

---

## Key Features

- ESP32-S3-MINI-1 module
- USB-C power and programming interface
- 5V to 3.3V voltage regulation
- Boot and reset circuitry
- WS2812B status LED
- ENS210 temperature sensor over I2C
- GPIO breakout headers
- 4-layer PCB design
- RF antenna keep-out consideration

---

## System Block Diagram

```text
USB-C Input
    │
    ├── ESD Protection
    │
    ├── 5V Power Rail ──> 3.3V Regulator ──> ESP32-S3-MINI
    │                                      ├── ENS210 Sensor
    │                                      ├── WS2812B LED
    │                                      └── GPIO Headers
    │
    └── USB Data Lines ──> ESP32-S3 USB Interface
