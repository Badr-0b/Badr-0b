# Badr Obtel

<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/0b3ae43d-b0a9-46cd-93ba-b550e904205b" />


Electrical Engineering student at AUM (Honors, Dean's List), entering junior year. I design embedded hardware, take digital designs from RTL to silicon, and build the software around them. Focus areas: PCB design, embedded firmware, and ASIC/VLSI.

Based in Kuwait. Open to remote internships and international roles in embedded systems, semiconductors, and edge hardware.

## What I do

**Hardware**
- PCB design in KiCad: schematic capture, layout, BOM, fab-ready Gerbers
- Embedded boards around ESP32 and STM32
- Power regulation, ESD protection, USB-C interfacing
- MIPI CSI-2 camera and multi-sensor (GNSS / IMU / magnetometer) interfacing

**Digital Design & Silicon**
- Verilog RTL design and self-checking verification
- Full open-source RTL-to-GDSII flow: Yosys, OpenROAD/LibreLane, Magic VLSI, KLayout, netgen
- SKY130 PDK, TinyTapeout packaging

**Firmware**
- C and C++ on ESP32 and STM32
- Peripherals: GPIO, PWM, SPI, I2C, UART, Wi-Fi, BLE
- STM32CubeMX, PlatformIO, Arduino core

**Software & Tooling**
- C, Python, Verilog
- Circuit simulation (OrCAD, LTSpice), 3D CAD (Fusion360)
- Supabase, Azure DevOps, Linux, Git

## Experience

### Software Engineering Intern, DevOps: Lear Corporation, E-Systems
*July 2026 to Aug 2026 | Sala Al Jadida, Morocco*

Build and release engineering for automotive electronic-systems validation.
- Re-architected a PowerShell hardware-in-the-loop test runner to execute cases in parallel, eliminating a hang that stalled validation runs for up to 5.5 hours and cutting a full pass to roughly 5 minutes.
- Designed and built CONDUIT, a local-first release-control dashboard unifying Azure DevOps with Palantir Foundry to auto-summarize deployment logs and replace a multi-page manual log-review workflow; adopted by full-time engineers.
- Debugged failing LIN-bus lighting and engine-cranking security-access test scripts across the CD TEST release pipeline, clearing the large majority of logged errors and restoring clean sign-off builds.
- Identified and patched a latent CI gate defect that passed pull requests with zero linked work items, closing a false-positive path that let unverified changes report as successful.

## Projects

### CLEAVE: RV32I Single-Cycle Core to SKY130 GDSII
*Verilog, Yosys, OpenROAD/LibreLane, Magic, sky130*

From-scratch RISC-V core hardened through a full open-source RTL-to-GDSII flow.
- Designed a from-scratch RV32I single-cycle processor core in Verilog implementing the full base integer ISA across a modular datapath: PC, 32x32 register file, ALU, immediate generator, branch comparator, control unit, and byte-addressable data memory.
- Hardened the RTL to a DRC/LVS-clean sky130 GDSII (Yosys synthesis; OpenROAD/LibreLane place-and-route and CTS; Magic/KLayout/netgen sign-off) at a 25 MHz target, packaged as a TinyTapeout 1x1 tile.
- Verified every module and the integrated core with 10 self-checking Icarus Verilog benches (9 unit plus a full-ISA integration proof) against hand-computed values through a debug port.

### NERONA: STM32N6 Computer Vision Edge Platform
*KiCad, STM32N6, MIPI CSI-2, STM32CubeMX*

Custom PCB targeting the STM32N6 NPU for on-device CV inference with no cloud dependency.
- Designed PCB power delivery, MIPI CSI-2 camera interface, and memory subsystem around the STM32N6 NPU for accelerated on-device inference.
- Completed schematic and layout in KiCad under signal-integrity and EMC rules, and built the deployment path for quantized object-detection models onto the NPU via STM32CubeMX.

### AZIMUTH: ESP32-S3 Multi-Sensor Navigation Board
*KiCad, ESP32-S3, GNSS, IMU, Sensor Fusion*

Custom navigation board with defined sensor roles and redundancy planning.
- Assigned each sensor a defined role: GNSS for position, magnetometer for heading, IMU accelerometer for tilt correction, and gyroscope for smoothing.
- Planned IMU dead-reckoning as a fallback for continuous heading and motion estimation during GNSS dropout.

## Looking for

Internships in embedded systems, semiconductors, IoT, or edge hardware with real ownership of PCB, firmware, power, or validation work.

## Contact

- LinkedIn: https://linkedin.com/in/badrobtel
- Email: badr@obtel.org

---

*Updated September 2026*
