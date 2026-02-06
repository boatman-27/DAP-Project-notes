The **PiSugar S Plus** is a compact, hardware-based **uninterruptible power supply (UPS)** designed for select Raspberry Pi models. It provides stable power delivery, seamless power switching, and basic power-state signaling without relying on software communication.

---
## Overview
- **Output:** 5V - 3A (continuous)
- **Battery Capacity:** 5000 mAh
- **UPS Functionality:** Yes (supports charge + discharge simultaneously)
- **Communication:** Hardware-only (no I²C battery telemetry)
- **Mounting:** Bottom-contact design (does not occupy GPIO header)
> ⚠️ PiSugar S Plus does **not** support Raspberry Pi 5B.
---
## Features
- $5V 3A$ output
- Bottom contact through pogo pins, so wont affect GPIO expansion
- Can be charges with TypeC & Micro USB charging
- Expansion support
	- Wireless charging
	- Solar charging (via add-ons)
---
## Functional Limitations
The PiSugar S Plus is **almost entirely hardware-based**, which leads to the following limitations:
- No I²C communication for:
    - Battery percentage
    - Voltage or current readings
    - Power statistics
- No scheduled power-on
---
## Supported Raspberry Pi Models
- Raspberry Pi 4B
- Raspberry Pi 3B
- Raspberry Pi 3B+
- Raspberry Pi 3A+
Raspberry Pi 5B is **not supported**
---
## Package Contents
- 1 × PiSugar S Plus battery module
- 4 × Mounting screws