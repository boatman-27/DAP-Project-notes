**PiSugar 3** is the third-generation battery and UPS module designed specifically for **Raspberry Pi Zero and Zero 2 (WH)** boards. It turns the Pi Zero into a truly portable system while adding software-controlled power management and an on-board **real-time clock (RTC)**.

---
## Overview
- **Form Factor:** Ultra-compact, back-contact design
- **Battery Capacity:** 1200 mAh
- **UPS Functionality:** Full UPS with soft shutdown support
- **Communication:** I²C (configurable address)
- **RTC:** On-board with write protection
---
## Features
- Full function **uninterruptible power supply (UPS)**
- Bottom contact through pogo pins, so wont affect GPIO expansion
- Can be charged with TypeC & Micro USB charging
- Hardware battery protection
	- PiSugar3 provides hardware charging protection function, which effectively improves battery cycle life.
- WebUI & APP
	- Mange PiSugar on your PC and mobile
---
### Software & Control
#### [[I²C]] Communication
- **Configurable I²C address**
    - Default: `0x57 / 0x68`
    - Address is mutable
- Enables:
    - Battery status reading
    - Voltage monitoring
    - Power control logic        
#### WebUI & Mobile App
- Manage PiSugar from:
    - PC browser
    - Mobile devices
- Monitor power status and configure behavior
#### OTA Firmware Upgrade
- Firmware updates without physical access
- Reduces maintenance friction
#### Software Watchdog
- Automatically restarts Raspberry Pi if:
    - System freezes
    - OS crashes
---
### On-board RTC (Real-Time Clock)
- Maintains correct system time when:
    - No power
    - No network access
- **Write-protected RTC**
    - Prevents data corruption
    - Guards against unstable system states or mis-operation
---
## Supported Raspberry Pi Models
- Raspberry Pi Zero (WH)
- Raspberry Pi Zero 2 (WH)

Not compatible with standard Raspberry Pi models (3B, 4B, 5B).

---
## Package Contents
- 1 × PiSugar 3 battery module (1200 mAh battery included)
- 4 × Mounting screws