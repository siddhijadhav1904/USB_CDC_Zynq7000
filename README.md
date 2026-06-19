# USB_CDC_Zynq7000
USB CDC implementation on Zynq-7000 (ZedBoard) enabling real-time Board-to-PC data transfer through a Virtual COM Port with Python-based data logging.
# USB CDC Communication on Zynq-7000 (ZedBoard)

## Overview

This project demonstrates the implementation of USB CDC (Communication Device Class) on the Xilinx Zynq-7000 SoC using the ZedBoard platform.

The system establishes a complete Board-to-PC communication pipeline where data generated on the embedded platform is transmitted over USB, enumerated as a Virtual COM Port on the host machine, and logged into a text file using a Python application.

---

## System Architecture

ZedBoard (Zynq-7000)
        │
        ▼
USB CDC Device
        │
        ▼
Virtual COM Port
        │
        ▼
Python (PySerial)
        │
        ▼
Text File Logging

---

## Hardware Platform

- Board: ZedBoard
- SoC: Xilinx Zynq-7000
- Toolchain:
  - Vivado 2023.1
  - Vitis 2023.1

---

## Features

- USB Device Mode Operation
- USB CDC Implementation
- Virtual COM Port Enumeration
- Continuous Data Streaming
- Host-Side Data Logging
- Embedded Firmware Development
- Hardware-Software Co-Design

---

## Implementation Flow

### Hardware Design

- Created Vivado Block Design
- Configured Zynq Processing System
- Enabled USB Peripheral in Device Mode
- Generated Bitstream
- Exported Hardware Platform (XSA)

### Software Development

- Developed USB CDC firmware in Vitis
- Initialized USB controller
- Implemented continuous data transmission
- Verified USB enumeration on Windows

### Host Application

- Developed Python application using PySerial
- Established communication through Virtual COM Port
- Logged incoming data into a text file

---

## Key Learnings

- USB CDC Architecture
- USB Enumeration Process
- Embedded Firmware Development
- Host-Device Communication
- Serial Data Logging
- Python Integration with Embedded Systems
- Zynq-7000 Development Flow

---

## Project Outcome

Successfully implemented an end-to-end embedded communication framework enabling reliable data transfer from the ZedBoard to a host PC through USB CDC.

The received data was captured through a Virtual COM Port and automatically stored in a text file for logging and analysis.

---

## Future Work

- Host → ZedBoard Communication
- Bidirectional USB CDC Data Exchange
- Command-Based Host Interface
- Real-Time Monitoring Applications
