# ACE Series

> **Professional Cycling Timing & Race Operations Platform**

ACE Series is an integrated platform designed for professional cycling events, providing accurate timing, race management, live results, and modular hardware integration.

The project aims to deliver a modern, flexible, and extensible ecosystem that supports multiple cycling disciplines while remaining independent of any specific hardware vendor.

---

# Vision

Our goal is to build an open and modular race timing platform that can be adapted to various cycling events and future technologies.

Instead of being tied to a single RFID vendor or timing solution, ACE Series is designed around standardized interfaces, allowing organizers to choose the hardware that best fits their needs.

---

# Supported Cycling Disciplines

- 🚴 Road Cycling
- 🚵 Mountain Bike (XCO / XCC / Marathon)
- 🚲 BMX Racing
- ⛰ Downhill (DH)
- ⏱ Individual Time Trial (ITT)
- 🔄 Circuit Race
- 🚴 Track Cycling (Planned)

---

# Core Philosophy

ACE Series is built on four key principles.

## Hardware Independent

The platform supports multiple hardware vendors through pluggable drivers.

Examples include:

- UHF RFID Readers
- Photo Finish Cameras
- Finish Capture Cameras
- LoRa Sensors
- Optical Sensors
- GPS Devices

---

## Modular Architecture

Every component operates independently.

```
ACE Series

├── ACE Core
│   ├── Event Bus
│   ├── API
│   ├── SDK
│   └── Plugin Framework
│
├── Circuit Race Manager
├── BMX Manager
├── Downhill Manager
├── Live Timing
├── Finish Capture
├── Finish Viewer
├── Judge Apps
├── Marshal Apps
└── Race Operations Platform
```

Each module can be developed, maintained, and deployed independently.

---

## Real-time Event Driven

Every hardware device produces standardized events.

```
RFID Reader
        │
Photo Finish
        │
LoRa Sensor
        │
Finish Camera
        │
GPS
        │
───────────────
ACE Core Event Bus
───────────────
        │
Race Manager
Live Timing
Result System
Judge UI
API
```

This architecture allows new hardware to be integrated without modifying the race management software.

---

# Key Features

## Professional Timing

- RFID Timing
- Finish Capture
- Photo Finish Integration
- Manual Backup Timing
- Optical Sensor Support

---

## Race Management

- Rider Registration
- Bib Management
- Category Management
- Heat Generation
- Random Gate Assignment
- Team Management
- Result Processing
- Time Penalties
- DNS / DNF / OTL Management

---

## Live Operations

- Live Timing
- TV Display
- Judge Dashboard
- Marshal Dashboard
- Mobile Applications
- Remote Monitoring

---

## Connectivity

- Ethernet
- TCP/IP
- USB
- LoRa
- REST API
- WebSocket

---

# RFID Integration

ACE Series does not depend on a single RFID manufacturer.

Supported hardware can be integrated through dedicated drivers.

Current evaluation includes:

- CHAFON
- INNOD
- Hopeland
- Impinj-based Readers

Future support will continue to expand.

---

# Finish Capture

ACE Series includes a dedicated Finish Capture module.

Features include:

- High FPS Camera Support
- Automatic Frame Capture
- Rider Identification
- Manual Verification
- Finish Viewer Integration

The Finish Capture module works together with RFID to improve race accuracy.

---

# Designed for Officials

ACE Series is developed with real race officials and organizers in mind.

The project focuses on reducing workload while improving accuracy and reliability during competitions.

---

# Future Roadmap

- AI-assisted Rider Detection
- Automatic Bib Recognition
- Multi-camera Finish Capture
- Cloud Synchronization
- Remote Event Monitoring
- Internationalization
- UCI Workflow Support
- Cross-platform Desktop Applications

---

# Open Architecture

ACE Series is designed to be extended.

Manufacturers and developers can integrate new devices using documented APIs and plugins.

The platform encourages interoperability rather than vendor lock-in.

---

# Project Status

Current Status:

✅ Core Architecture Design

✅ Desktop Applications

✅ Race Management

🚧 RFID Integration

🚧 Finish Capture

🚧 Live Timing

🚧 Judge Mobile Applications

---

# Contact

ACE Series Development

Republic of Korea

For technical collaboration, hardware integration, or partnership inquiries, please feel free to contact us.
