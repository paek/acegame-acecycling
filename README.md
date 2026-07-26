# 🚴 ACE Series

> **Any Hardware. One Platform.**
>
> **모든 계측 기술을 하나의 플랫폼으로.**

---

> [!IMPORTANT]
>
> ## 📖 문서 정책 (Documentation Policy)
>
> 본 문서는 **ACE Series의 공식 한국어 문서(Official Source)** 입니다.
>
> `README.en.md`를 포함한 모든 영어 문서는 한국어 원본을 기반으로 작성되는 **공식 번역본(Official Translation)** 입니다.
>
> 문서 간 내용이 상이한 경우에는 **한국어 문서를 기준**으로 합니다.

---

# ACE Series란?

ACE Series는 단순한 경기 계측 프로그램이 아닙니다.

ACE Series는 **사이클 경기 운영과 계측을 위한 하드웨어 독립형(Hardware Independent) 플랫폼**입니다.

기존의 대부분의 계측 시스템은 특정 제조사의 장비와 소프트웨어가 하나의 제품으로 구성됩니다.

ACE Series는 이러한 구조에서 벗어나 다양한 계측 기술과 다양한 제조사의 장비를 하나의 플랫폼에서 통합하여 사용할 수 있도록 설계되었습니다.

즉,

**하드웨어는 교체할 수 있지만 플랫폼은 유지됩니다.**

---

# 프로젝트 비전

ACE Series의 목표는 매우 단순합니다.

> **어떤 계측 장비라도 하나의 플랫폼에서 사용할 수 있도록 한다.**

RFID

Active Transponder

Photo Finish

Finish Capture

LoRa

Optical Sensor

GPS

그리고 앞으로 등장할 새로운 계측 기술까지.

ACE Series는 특정 기술을 위한 프로그램이 아니라 **모든 계측 기술을 위한 플랫폼**을 목표로 합니다.

---

# 왜 ACE Series인가?

현재 대부분의 경기 계측 시스템은 다음과 같은 구조를 가지고 있습니다.

```text
MYLAPS
    │
MYLAPS Software

Race Result
    │
Race Result Software

RFID Reader
    │
Vendor Software
```

장비가 변경되면 소프트웨어도 함께 변경됩니다.

ACE Series는 반대로 생각합니다.

```text
                Timing Technologies

 RFID
 Active Transponder
 Photo Finish
 Finish Capture
 Optical Sensor
 LoRa
 GPS
 Manual Timing

                 │

                 ▼

             ACE Core

                 │

       Race Management Platform

                 │

 Live Timing
 Judge
 Marshal
 Results
 API
 Viewer
```

계측 기술은 언제든 변경될 수 있습니다.

그러나 경기 운영 플랫폼은 변경되지 않아야 합니다.

---

# 핵심 철학

ACE Series는 다음 다섯 가지 철학을 기반으로 설계됩니다.

## Hardware Independent

특정 제조사에 종속되지 않습니다.

MYLAPS가 될 수도 있고

CHAFON이 될 수도 있으며

새로운 제조사가 등장하더라도 플랫폼은 그대로 유지됩니다.

---

## Timing Technology Independent

RFID만을 위한 프로그램이 아닙니다.

Transponder만을 위한 프로그램도 아닙니다.

ACE Series는 **계측 기술 자체를 추상화(Abstract)** 합니다.

모든 계측 기술은 하나의 Timing Source로 동작합니다.

---

## Event Driven

모든 장비는 이벤트를 생성합니다.

ACE Core는 이벤트만 처리합니다.

장비의 종류는 중요하지 않습니다.

---

## Modular

ACE Series는 하나의 거대한 프로그램이 아닙니다.

필요한 기능만 독립적으로 개발하고 배포할 수 있는 모듈형 플랫폼입니다.

---

## Open Architecture

새로운 장비가 출시되더라도

ACE Core를 수정하지 않고

Plugin 또는 Driver만 추가하여 사용할 수 있도록 설계됩니다.

---

# 지원 경기 종목

ACE Series는 다양한 사이클 종목을 지원하도록 설계됩니다.

- 🚴 Road Cycling
- 🚵 Mountain Bike (XCO)
- 🚵 Mountain Bike (XCC)
- 🚵 Marathon (XCM)
- 🚲 BMX Racing
- ⛰ Downhill (DH)
- 🛣 Individual Time Trial (ITT)
- 🔄 Circuit Race
- 🚴 Track Cycling *(Planned)*

---

# 지원 계측 기술

ACE Series는 하나의 계측 기술에 종속되지 않습니다.

## Commercial Timing Systems

- MYLAPS
- Race Result
- TAG Heuer Timing
- ChronoTrack
- 기타 상용 계측 시스템

---

## RFID

- Passive UHF RFID
- Multi Reader
- Multi Antenna

---

## Active Transponder

- Active RFID
- Decoder Based Systems
- Professional Timing Systems

---

## Camera Based Timing

- Finish Capture
- Photo Finish
- High-Speed Camera

---

## Sensor Based Timing

- Optical Sensor
- LoRa Node
- GPS Device
- BLE Device
- Manual Timing

---

# 플랫폼 구성

```text
ACE Series

├── ACE Core
│
├── Circuit Race Manager
├── MTB Manager
├── BMX Manager
├── Downhill Manager
│
├── Finish Capture
├── Finish Viewer
│
├── Live Timing
│
├── Judge App
├── Marshal App
│
└── Race Operations Platform
```

모든 모듈은 독립적으로 개발되고 유지됩니다.

---

# 문서 구성

ACE Series는 코드보다 문서를 우선하는 프로젝트를 지향합니다.

현재 작성 중인 공식 문서는 다음과 같습니다.

| 문서 | 설명 |
|------|------|
| README.md | 프로젝트 소개 |
| MANIFESTO.md | 프로젝트 선언문 |
| DESIGN_PRINCIPLES.md | 설계 원칙 |
| ARCHITECTURE.md | 전체 아키텍처 |
| TIMING_SOURCES.md | 계측 기술 추상화 |
| EVENT_BUS.md | Event Bus 구조 |
| HARDWARE.md | 지원 하드웨어 |
| API.md | API 명세 |
| PLUGIN_SDK.md | Plugin 개발 가이드 |
| ROADMAP.md | 개발 계획 |
| GLOSSARY.md | 용어집 |

---

# 현재 개발 상태

| 구성 요소 | 상태 |
|-----------|------|
| ACE Core | 🚧 개발 중 |
| Circuit Race Manager | 🚧 개발 중 |
| RFID | 🚧 개발 중 |
| Active Transponder | 📋 계획 |
| Finish Capture | 🚧 개발 중 |
| Live Timing | 🚧 개발 중 |
| Judge App | 🚧 개발 중 |
| Marshal App | 📋 계획 |
| Cloud Services | 📋 계획 |

---

# 앞으로의 목표

ACE Series는 단순한 경기 운영 프로그램이 아닌,

국제대회부터 지역 대회까지 사용할 수 있는 **개방형 사이클 계측 플랫폼(Open Cycling Timing Platform)** 을 목표로 합니다.

새로운 계측 기술이 등장하더라도 플랫폼은 그대로 유지될 수 있도록 지속적으로 발전해 나갈 예정입니다.

---

# 프로젝트 슬로건

> **Any Hardware. One Platform.**

> **하드웨어는 바뀔 수 있습니다.**

> **기술은 발전합니다.**

> **플랫폼은 흔들리지 않아야 합니다.**

---

# Contact

**ACE Series Development**

Republic of Korea

기술 협업, 하드웨어 연동, SDK 개발 또는 파트너십에 관심이 있으시다면 언제든지 연락해 주시기 바랍니다.
