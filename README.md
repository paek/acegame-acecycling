# ACE Series

<div align="center">

# 🚴 ACE Series

### Professional Cycling Timing & Race Operations Platform

*A hardware-independent, modular platform for professional cycling events.*

---

Road Cycling • MTB • BMX • Downhill • Track Cycling • Time Trial

</div>

---

# Overview

ACE Series is a next-generation race timing and race operations platform designed specifically for cycling competitions.

Unlike traditional timing systems that rely on a single hardware vendor, ACE Series is designed around an open and modular architecture that supports multiple timing technologies and hardware manufacturers.

The platform combines timing, race management, live timing, finish verification, mobile applications, and hardware integration into a single ecosystem.

---

# Vision

Our vision is to build an open, extensible and hardware-independent timing platform for professional cycling.

ACE Series is designed to allow organizers to choose the most suitable hardware without changing their race management software.

Rather than locking users into a single RFID or transponder vendor, ACE Series provides standardized interfaces for integrating multiple timing technologies.

---

# Supported Disciplines

- 🚴 Road Cycling
- 🚵 Cross Country (XCO)
- 🚵 Cross Country Short Track (XCC)
- 🚵 Marathon (XCM)
- 🚲 BMX Racing
- ⛰ Downhill (DH)
- 🛣 Individual Time Trial (ITT)
- 🔄 Circuit Race
- 🚴 Track Cycling *(Planned)*

---

# Core Philosophy

ACE Series is built around five core principles.

---

## 1. Hardware Independent

ACE Series is **not tied to a single hardware vendor**.

Supported hardware can be added through modular drivers.

Examples include:

- Passive RFID Readers
- Active Transponder Systems
- Photo Finish Systems
- High-Speed Finish Cameras
- Optical Timing Sensors
- LoRa Timing Nodes
- GPS Timing Devices
- Manual Timing Consoles

---

## 2. Timing Technology Independent

ACE Series supports multiple timing technologies.

```
Timing Sources

├── Passive RFID
├── Active Transponder
├── Finish Capture
├── Photo Finish
├── Optical Sensor
├── LoRa Sensor
├── GPS Timing
└── Manual Timing
```

All timing sources generate a common event format inside ACE Core.

---

## 3. Event-Driven Architecture

Every connected device publishes standardized events.

```
RFID Reader
Active Transponder
Photo Finish
Finish Capture
LoRa Sensor
Optical Sensor
GPS

        │
        ▼

  ACE Core Event Bus

        │

Race Manager
Live Timing
Judge UI
Results
API
```

The race management software never communicates directly with hardware.

---

## 4. Modular Design

Every component operates independently.

```
ACE Series

├── ACE Core
│   ├── Event Bus
│   ├── API
│   ├── SDK
│   ├── Plugin Framework
│   └── Device Manager
│
├── Circuit Race Manager
├── BMX Manager
├── MTB Manager
├── Downhill Manager
├── Finish Capture
├── Finish Viewer
├── Live Timing
├── Judge Application
├── Marshal Application
└── Race Operations Platform
```

Each module can evolve independently while sharing the same core.

---

## 5. Open Integration

ACE Series is designed for interoperability.

Manufacturers can integrate their own hardware by implementing a timing driver without modifying the core platform.

---

# Timing Technologies

## Passive RFID

Designed for affordable and flexible race timing.

Features:

- EPC Gen2
- Multi Reader Support
- Multi Antenna Support
- TCP/IP Communication
- USB Communication
- Reader Abstraction Layer

Current evaluation:

- CHAFON
- Hopeland
- INNOD
- Impinj Based Readers

---

## Active Transponder

Designed for professional timing systems.

Planned support includes:

- Multi-channel Detection
- High-speed Racing
- Long Range Detection
- Multiple Decoder Support
- Professional Timing Systems

Examples:

- Road Cycling
- MTB
- BMX
- Running
- Triathlon
- Motorsport

---

## Finish Capture

ACE Finish Capture is a dedicated video-assisted finish verification system.

Features:

- High FPS Cameras
- Automatic Image Capture
- Rider Identification
- Manual Verification
- Finish Viewer Integration

---

## Photo Finish

Support for professional photo finish systems.

Planned features:

- Image Synchronization
- Timing Synchronization
- External Photo Finish Integration
- Result Verification

---

## Optical Sensors

Support for:

- Laser Sensors
- Infrared Beam Sensors
- Photoelectric Sensors
- Start Gate Sensors

---

## LoRa Timing Network

Designed for remote timing locations.

Examples:

- Intermediate Split
- Downhill Start
- Feed Zone
- Mountain Checkpoint
- Remote Timing Stations

---

## Manual Timing

ACE Series always supports manual timing as a backup solution.

Manual timing events are integrated into the same event processing pipeline.

---

# Race Management

ACE Series provides comprehensive race management tools.

Features include:

- Rider Registration
- Category Management
- Team Management
- Bib Assignment
- Heat Generation
- Random Gate Assignment
- Qualification
- Seeding
- DNS
- DNF
- OTL
- Time Penalties
- Result Processing

---

# Live Operations

Real-time race operations include:

- Live Timing
- Judge Dashboard
- Marshal Dashboard
- TV Display
- Mobile Applications
- Race Control
- Event Monitoring

---

# Connectivity

Supported communication methods include:

- Ethernet
- TCP/IP
- USB
- Serial (RS232 / RS485)
- LoRa
- REST API
- WebSocket
- Local Event Bus

---

# Hardware Architecture

```
Timing Hardware

RFID Reader
Active Transponder
Photo Finish
Finish Capture
Optical Sensor
LoRa Node

        │

Device Driver

        │

ACE Core

        │

Race Manager

        │

Results
Live Timing
Judge UI
API
```

The platform is designed so that hardware can be replaced without changing race management software.

---

# Designed for Officials

ACE Series is developed by active cycling officials with practical experience in race operations.

The focus is on:

- Reliability
- Simplicity
- Accuracy
- Speed
- Expandability

---

# Future Roadmap

Planned developments include:

- AI Rider Detection
- Automatic Bib Recognition
- Multi Camera Finish Capture
- Cloud Synchronization
- Internationalization
- UCI Workflow Support
- Cross Platform Applications
- Hardware SDK
- Third-party Plugin SDK

---

# Current Status

| Module | Status |
|----------|--------|
| ACE Core | 🚧 In Development |
| Race Manager | 🚧 In Development |
| RFID Integration | 🚧 Evaluation |
| Active Transponder | 📋 Planned |
| Finish Capture | 🚧 In Development |
| Photo Finish Integration | 📋 Planned |
| Live Timing | 🚧 In Development |
| Judge App | 🚧 In Development |
| Marshal App | 📋 Planned |

---

# Philosophy

> Hardware should never dictate software.

ACE Series separates race management from timing hardware, allowing organizers to choose the best solution for every event.

Our goal is to build an open ecosystem for professional cycling timing.

---

# Contact

**ACE Series Development**

Republic of Korea

For technical collaboration, hardware integration, or partnership inquiries, please feel free to contact us.
