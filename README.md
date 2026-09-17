# DC-Motor-Speed-Controller

A compact, high-efficiency Pulse Width Modulation (PWM) DC motor speed controller circuit designed for precise speed and directional control of brushed DC motors.
---

## 🚀 Features

- **PWM Speed Control:** Smooth variable speed adjustment using a high-frequency PWM signal (adjustable via potentiometer or external microcontroller input).
- **High-Current Handling:** Designed with robust MOSFET drivers to support continuous high current loads with minimal thermal loss.
- **Directional Control:** Integrated H-Bridge configuration (or relay/logic control) for forward, reverse, and braking capabilities.
- **Onboard Protection:** 
  - Reverse polarity protection on the power input.
  - Flyback diodes to prevent inductive voltage spikes.
  - Overcurrent / thermal protection fuse.
- **LED Indicators:** Visual status indicators for power, operational state, and fault conditions.

---

## 🛠️ Hardware Specifications

| Parameter | Specification |
| :--- | :--- |
| **Input Voltage ($V_{in}$)** | 12V – 24V DC |
| **Max Continuous Current** | 10A (with proper heatsinking) |
| **PWM Frequency** | 1kHz – 20kHz |
| **Control Signal** | 0–5V analog or 3.3V/5V TTL PWM |
| **PCB Dimensions** | 50mm x 70mm (Double-layer) |

---
Getting Started & Assembly
Fabrication:

Download the production files from the hardware/gerbers/ folder and send them to your preferred PCB manufacturer.

Assembly (BOM):

Refer to the Bill of Materials (docs/BOM.csv) for component values.

Solder passive components (resistors, capacitors, diodes) first, followed by ICs, connectors, and power MOSFETs. Ensure power MOSFETs are mounted with adequate heatsinking if operating near maximum current limits.

Testing:

Double-check all power lines for short circuits using a multimeter before connecting power.

Connect a regulated DC power supply to VIN+ and GND.

Connect your brushed DC motor to MOT+ and MOT-.

Adjust the onboard potentiometer or apply a PWM signal to verify smooth speed variation.
