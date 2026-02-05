Short for (Inter-Integrated Circuit), is a popular, two wire serial communication protocol for short-distance communication between microcontrollers and peripheral chips (like sensors, and memory) on a circuit board. 

It uses two wires, 
1. Serial Data (SDA) -> Carries actual data
2. Serial Clock (SCL) -> Controls the timing of data transfer

## How it works
 - **Two wires:** Data (SDA) and clock (SCL)
 - **Synchronous:** A shared clock to ensure that data is synchronised
 - **Multi-Master/Multi-Slave:** Multiple controllers (masters) and devices (slaves) can connect to the same bus
 - **Addressing:** Each slave device has a unique address
 - **Master-Driven:** A master initiates communication, sends the slave's address, and manages data flow (reading/writing)
## Uses
- Connecting sensors, displays, EEPROMs, RTCs to microcontrollers (like Arduino, ESP32).
- IoT, consumer electronics, industrial automation. 

## Benefits
- **Simplicity:** Only two wires needed.
- **Flexibility:** Easy to add multiple devices.
- **Cost-Effective:** Reduces pin usage on microcontrollers.

### What actually happens (step by step)

1. **Software** (an app, daemon, or kernel driver) wants information  
    Example: battery percentage.
2. Software talks to the **CPU**  
    (because software always does)
3. The CPU uses its **I²C controller**  
    This is hardware inside the CPU/SoC.
4. The CPU **asks the component** over I²C  
    Example:  
    “Device at address `0x57`, give me register 0x02.” (register is a specific, internal storage location within slave device)
5. The **component replies** over I²C  
    It sends back raw data.
6. The CPU receives the data
7. **Software interprets it**
    - 0x64 → 100% battery
    - 0x01 → charging
    - etc.
8. Software decides what to do
    - show battery icon
    - log it
    - shut down safely