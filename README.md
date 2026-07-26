<div align="center">

# 🚴 ACE Series

## Any Hardware. One Platform.

### Vendor-Independent Cycling Timing Platform

Professional Timing • Race Operations • Live Timing • Finish Capture

Road Cycling • MTB • BMX • Downhill • Track Cycling

---

**Build Once. Integrate Everything.**

</div>

---

# About

ACE Series is an open and modular timing platform designed for professional cycling competitions.

Unlike traditional timing software that depends on a specific hardware vendor, ACE Series separates race management from timing hardware through a unified event-driven architecture.

Whether timing data comes from RFID, active transponders, photo finish systems, cameras, optical sensors, or future technologies, the race management software remains exactly the same.

The hardware can change.

The platform does not.

---

# Vision

Our vision is simple.

> Any Hardware. One Platform.

ACE Series aims to become an open timing platform capable of integrating commercial timing systems, open hardware, and future technologies into a single ecosystem.

Instead of replacing existing timing systems, ACE Series connects them.

---

# Core Principles

## Hardware Independent

ACE Series is designed to work with multiple hardware vendors.

Examples include:

- MYLAPS
- Race Result
- TAG Heuer Timing
- ChronoTrack
- CHAFON
- Zebra
- Hopeland
- Impinj-based Readers
- Custom Devices

No single vendor is required.

---

## Timing Technology Independent

Timing technology should never dictate software architecture.

ACE Series supports multiple timing technologies simultaneously.

```
Timing Technologies

├── Passive RFID
├── Active Transponder
├── Photo Finish
├── Finish Capture
├── Optical Timing
├── LoRa Timing
├── GPS Timing
├── Manual Timing
└── Future Technologies
```

Every timing technology is treated as a timing source.

---

## Event Driven

Every timing source generates standardized timing events.

```
          Timing Sources

RFID
MYLAPS
Race Result
Photo Finish
Finish Capture
LoRa
GPS
Manual Timing

          │

          ▼

   ACE Core Event Bus

          │

 Race Manager
 Live Timing
 Results
 Judge UI
 REST API
 WebSocket
```

Hardware never communicates directly with the race management software.

---

## Modular

```
ACE Series

├── ACE Core
│   ├── Event Bus
│   ├── Plugin Framework
│   ├── Timing SDK
│   ├── Device Manager
│   └── API
│
├── Circuit Race Manager
├── MTB Manager
├── BMX Manager
├── Downhill Manager
├── Finish Capture
├── Finish Viewer
├── Live Timing
├── Judge App
├── Marshal App
└── Race Operations Platform
```

Every module can evolve independently.

---

# Timing Sources

ACE Series supports multiple timing technologies through a common interface.

```
ITimingSource

├── RFID Reader
├── Active Transponder
├── Photo Finish
├── Finish Capture
├── Optical Sensor
├── LoRa Sensor
├── GPS Device
└── Manual Timing
```

All timing sources generate the same event structure.

```
TimingEvent

Timestamp

Participant

Source

Location

RSSI / Signal

Metadata
```

This allows race management software to remain hardware-independent.

---

# Supported Disciplines

- Road Cycling
- Mountain Bike
- BMX Racing
- Downhill
- Individual Time Trial
- Circuit Race
- Track Cycling *(Planned)*

---

# Commercial Timing Integration

ACE Series is designed to integrate with existing commercial timing systems.

Examples include:

- MYLAPS
- Race Result
- TAG Heuer Timing
- ChronoTrack
- Professional Photo Finish Systems

Commercial timing hardware remains the property of its respective manufacturers.

ACE Series acts as an integration platform rather than replacing those systems.

---

# Open Hardware Support

ACE Series also supports vendor-independent hardware.

Examples:

Passive RFID

- CHAFON
- Hopeland
- Zebra
- Impinj Based Readers

Custom Transponder Systems

Finish Capture Cameras

Optical Sensors

LoRa Nodes

GPS Devices

---

# Finish Capture

ACE Finish Capture is an integrated finish verification system.

Features include:

- High-speed cameras
- Automatic frame capture
- Rider verification
- Manual review
- Finish Viewer

Designed to complement RFID and transponder timing.

---

# Live Operations

ACE Series provides:

- Live Timing
- Judge Dashboard
- Marshal Dashboard
- TV Display
- Mobile Applications
- Event Monitoring
- Race Control

---

# Connectivity

Supported interfaces include:

- TCP/IP
- Ethernet
- USB
- RS232
- RS485
- WebSocket
- REST API
- LoRa
- Bluetooth
- Serial Communication

---

# Designed by Officials

ACE Series is developed by active cycling officials.

Every feature is based on real race operation experience.

The project prioritizes:

- Reliability
- Accuracy
- Simplicity
- Expandability

---

# Roadmap

Current Development

✅ ACE Core

🚧 Race Manager

🚧 RFID

🚧 Active Transponder

🚧 Finish Capture

🚧 Live Timing

🚧 Judge App

📋 Marshal App

📋 Cloud Services

📋 AI Rider Recognition

---

# Open Architecture

ACE Series encourages hardware manufacturers and developers to integrate their products through documented APIs and plugins.

The goal is to build an open ecosystem for professional cycling timing.

---

# Philosophy

> Hardware evolves.

> Timing technologies change.

> Competition rules evolve.

**The platform should not have to be rewritten every time.**

ACE Series separates race management from timing hardware, allowing organizers to adopt new technologies without rebuilding their entire software ecosystem.

---

# License

Project License: TBD

---

# Contact

ACE Series Development

Republic of Korea

For collaboration, hardware integration, SDK development or partnership opportunities, please feel free to contact us.
