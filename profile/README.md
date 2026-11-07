<div align="center">

# Coreforge Systems

### Industrial software for machines, embedded devices, and service teams.

**Reliable C++/Qt solutions for device diagnostics, configuration, telemetry, automation, and industrial service workflows.**

</div>

---

## About Coreforge Systems

Coreforge Systems develops software for industrial machines, embedded devices, and engineering teams.

Our focus is on software that connects directly to physical equipment and helps engineers configure devices, diagnose failures, inspect telemetry, analyze machine state, and perform service operations more efficiently.

We build systems around a simple principle:

> **Industrial software should make complex equipment easier to understand, diagnose, and maintain.**

Our primary areas of interest include:

- Industrial device diagnostics
- Embedded device configuration
- Machine telemetry and monitoring
- Service and maintenance tooling
- Industrial communication protocols
- Production testing
- Hardware/software integration
- Machine connectivity

---

## Current Project

### DevicePilot

**DevicePilot** is our primary project currently under development.

It is an OEM-oriented service and diagnostics platform designed for manufacturers of industrial machines and embedded equipment.

DevicePilot provides a unified desktop environment for:

- Device identification
- TCP and Serial communication
- Configuration management
- Parameter validation
- Live telemetry
- Equipment diagnostics
- Event logging
- Configuration snapshots
- Configuration comparison
- Support package generation
- Guided troubleshooting
- Service workflows

The goal is to give machine manufacturers and their service engineers a single tool for diagnosing and maintaining equipment installed at customer sites.

### Typical workflow

```text
Industrial Machine
        │
        ▼
Controller / Embedded Device
        │
        ▼
TCP / Serial / Industrial Protocol
        │
        ▼
DevicePilot
        │
        ├── Device Identification
        ├── Configuration
        ├── Telemetry
        ├── Diagnostics
        ├── Troubleshooting
        └── Support Reports
```

DevicePilot is currently in active development.

---

## Engineering Focus

Our software is primarily built around modern C++ and Qt.

### Core technologies

```text
C++20
Qt 6
CMake
Linux
Windows
TCP/IP
Serial Communication
SQLite
Embedded Systems
```

### Embedded & Hardware

```text
ESP32
STM32
Embedded Linux
Sensors
Controllers
Industrial Devices
```

### Industrial communication

Current development focuses on:

```text
TCP
Serial / UART
Custom binary protocols
```

Future integrations may include:

```text
Modbus TCP / RTU
OPC UA
CAN
MQTT
```

Protocol support is added based on real industrial use cases rather than simply increasing the number of supported technologies.

---

## Architecture

Our software follows a modular architecture designed to isolate device-specific functionality from reusable platform components.

```text
Presentation
     │
     ▼
Application Services
     │
     ▼
Device Sessions
     │
     ▼
Operation Scheduler
     │
     ├── Configuration
     ├── Telemetry
     ├── Diagnostics
     └── Reporting
     │
     ▼
Device Adapter
     │
     ▼
Protocol Codec
     │
     ▼
Transport
     │
     ├── TCP
     └── Serial
     │
     ▼
Physical Device
```

The objective is to allow support for new machines and controllers without rebuilding the entire application architecture.

---

## Engineering Principles

### Reliability first

Industrial software must continue behaving predictably when:

- connections are unstable;
- devices stop responding;
- packets are corrupted;
- operations time out;
- equipment returns unexpected data.

Failure handling is considered part of the normal application workflow.

### Read-only by default

Diagnostic operations should not modify machine state unless an operation explicitly requires it.

### Hardware-independent core

Communication infrastructure, diagnostics, reporting, and UI should remain reusable across multiple device families.

Device-specific behaviour belongs in dedicated adapters.

### Test without hardware

Every supported device integration should be testable using simulators and protocol tests without requiring physical equipment for every development cycle.

### Explicit state

Applications should always distinguish between:

```text
Confirmed
Rejected
Unknown
Unavailable
```

For industrial systems, an unknown result must never be presented as a successful operation.

---

## Simulation & Testing

DevicePilot development includes simulated industrial devices capable of reproducing both normal behaviour and communication failures.

Simulation scenarios include:

```text
Normal device operation

Connection timeout

Unexpected disconnect

Delayed response

Invalid packet

Checksum failure

Device busy

Invalid parameter

Sensor failure

Controller failure
```

This allows communication and diagnostic workflows to be tested before connecting to real industrial hardware.

Physical validation is performed using embedded development hardware such as ESP32-based devices.

---

## What We Are Building Towards

Coreforge Systems aims to build reusable engineering tools for machine manufacturers and industrial technology companies.

Our long-term product direction includes:

```text
Coreforge Systems

├── DevicePilot
│   Device diagnostics & service platform
│
├── Device Integration SDK
│   Integration of new controllers and machines
│
├── Production Test Tools
│   Automated device and manufacturing testing
│
└── Industrial Connectivity Tools
    Communication, protocol and telemetry tooling
```

We are deliberately focused on solving specific industrial engineering problems rather than building a generic IoT or SCADA platform.

---

## Project Status

**DevicePilot:** Active development

Current development priorities:

- Core architecture
- Device communication layer
- TCP device simulator
- Protocol implementation
- Device sessions
- Operation scheduling
- Configuration management
- Diagnostics
- Support package generation
- ESP32 hardware emulator
- Automated testing

---

## Coreforge Systems

**Industrial software for connected machines, embedded devices, diagnostics, and automation.**
