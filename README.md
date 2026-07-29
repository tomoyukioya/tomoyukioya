[日本語](README.ja.md)

# Software Portfolio

Rooted in R&D in broadcasting and telecommunications, I design and implement across **video, 3D measurement, embedded systems, and distributed processing** — end to end, from close-to-hardware layers up to applications. My primary language is **C# / .NET**; I also use C/C++, Python, and Kotlin daily.

![C#](https://img.shields.io/badge/C%23-239120?style=flat&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat&logo=dotnet&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white)

---

## Focus Areas

- **Broadcast & Video** — MPEG2-TS / ARIB standards / HLS streaming
- **3D & Measurement** — LiDAR & point clouds (LAS / LAZ) / sensors / AR
- **Embedded & Payment Terminals** — Android embedded / FeliCa・NFC / cashless payments
- **Cloud & Distributed Processing** — AWS / distributed rendering
- **Wireless & Radio** — Local 5G / radio-wave propagation & coverage
- **Business Systems & Automation** — WPF・WinForms / Blazor / scraping・RPA

---

## Selected Products

### Broadcast & Video
- **MPEG2-TS analysis/repair engine + HLS delivery platform** — Conforms to ARIB STD-B10 / B24 / B25. Detects and repairs TOT/PCR inconsistencies originating from live broadcast waves, through to iOS/Android playback. Maintained over the long term.
- **TS merge/repair toolset** (tsrepair / PcrCheck / TotDupCheck / TotGapCheck, etc.) — C/C++.
- **Closed-caption extraction tool (ARIB STD-B24)** and a **C# implementation of BonDriver**.
- **HLS video downloader** — WebView2 + ffmpeg.

### 3D & Measurement
- **LiDAR point-cloud processing / LAS・LAZ 1.4 parser** — Built a **custom C# wrapper for PDAL** to use it from .NET.
- **Parser for Livox's proprietary binary (LVX)** and a **multi-pane point-cloud viewer** (OpenGL).
- **SignalR-based real-time communication backbone**, **IoT measurement** (tide sensors), an **AR display server**, and a **3D TOF sensor app** (WPF).

### Embedded & Payment Terminals
- **Android embedded-device apps** — Built for kiosk operation and SIP calling; extended to watch-over / care-robot use.
- **Unattended-retail & payment-terminal apps** — FeliCa / NFC / credit-card payments / Adyen / Mobile Suica. Signed-APK distribution, alcohol-sales compliance, and more.

### Cloud & Distributed Processing
- **Cloud rendering platform (server side)** — Supports Maya / Blender / Arnold / V-Ray / ProRender. AWS S3 integration, distributed rendering, a CLI edition, and GPU-type / server-count selection, developed continuously.

### Wireless & Radio
- **Local-5G coverage-calculation app** — Coverage computation and map rendering using ITU-R P.526 / F.1336 and GSI DEM / PLATEAU. Generates existing-coverage areas from license data to visualize interference (GPU-accelerated).
- **LTE / 5G(NSA) drive-test measurement system** — Kotlin / Chaquopy / Python / FastAPI / Leaflet. Qualcomm diagnostic logs, RM520N-GL + Raspberry Pi 4B.

### Business Systems & Automation
- **Property-information management app for real estate** — Property management, automated portal entry, and automatic selection/generation of contract templates. Roughly **34,000 lines with 167 unit tests**. .NET 8 / EF Core / WebView2 / GPT-4o.
- **License-authentication platform** — Server + resident service + embedded library + admin console. Blazor Server / ASP.NET Core Identity / RSA-2048・SHA-256 / obfuscation for tamper resistance.
- **FPGA update and host-control software for a high-speed A/D board** — 200 MSPS support. Register control (ADS5295 / LMK04610, etc.), DDR3・FIFO capture, and a waveform viewer (with bin→CSV conversion).
- **Mail-distribution & contact-list tools**, and **cross-site data-collection tools** (WebView2 scraping).

### Web & PWA
- **PWA for field/visiting staff** (Blazor / PWA / Push Notification), plus backend and CRM development and improvements.

### Distributed Ledger & Trading
- **ERC token issuance with a portal** (Ethereum / geth / smart contracts) and **exchange-API trading bots** (Python / BitMEX, etc.).

---

## Open-Source Software

| Repository | Language | License | Description |
|---|---|---|---|
| [FileHistoryClone](https://github.com/tomoyukioya/FileHistoryClone) | C# | MIT | Resident, generational backup tool in the spirit of File History (`winget install tomoyukioya.FileHistoryClone`) |
| [WiFiArea](https://github.com/tomoyukioya/WiFiArea) | C# | MIT | Indoor Wi-Fi coverage simulator based on ITU-R recommendations (combines path loss, wall transmission, and diffraction) |
| [SmartPhoneCTI](https://github.com/tomoyukioya/SmartPhoneCTI) | C# | MIT | CTI that surfaces smartphone incoming calls as PC desktop notifications (three-tier) |
| [WinKvm](https://github.com/tomoyukioya/WinKvm) | C# | MIT | Software KVM console using a CH9329 USB HID (can even operate BIOS/UEFI screens) |
| [TH850Library](https://github.com/tomoyukioya/TH850Library) | C# | MIT | Access library for a USB pedometer |
| [CheckScreenColor](https://github.com/tomoyukioya/CheckScreenColor) | C# | Apache-2.0 | Monitors screen pixels and notifies on a specific color |
| [MicroOvenCalc](https://github.com/tomoyukioya/MicroOvenCalc) | HTML/JS | — | Microwave heating-time calculator |

---

## Tech Stack

- **Languages**: C# / C・C++ / Python / Kotlin・Java / JavaScript
- **.NET**: WPF・WinForms / ASP.NET Core / Blazor / EF Core
- **Cloud & Infra**: AWS (S3・Lambda・WAF) / Azure (App Service・DevOps)
- **Data**: SQL Server / SQLite / LiteDB
- **Domain**: MPEG2-TS・ARIB / HLS / LiDAR & point clouds (LAS・LAZ) / FeliCa・NFC・payments / SignalR / MQTT / ITU-R radio propagation

---

## Background

I have spent many years in R&D across broadcasting and telecommunications, including the operation of broadcast and information systems and hands-on security operations covering conditional-access systems (CAS). Today's software work builds on that foundation in hardware, communications, and security.
