# Somnus v1.0.0

## Smart Sleep Stage Monitor & Intelligent Wake System

The **Somnus v1.0.0** release brings together the core hardware, firmware, machine learning, backend, and frontend components into a unified sleep monitoring system.

Somnus uses ECG signals to analyze sleep patterns, classify sleep stages, and provide intelligent wake functionality through a connected monitoring dashboard.

## What's Changed

- Introduced **ECG-based sleep monitoring** using the AD8232 and ESP32.
- Added **250 Hz ECG signal acquisition**.
- Added **Pan–Tompkins R-peak detection** and RR interval extraction.
- Added **HRV feature extraction** for sleep analysis.
- Added lightweight **XGBoost-based sleep-stage classification** with ONNX Runtime.
- Added **NREM, REM, and Wake** classification.
- Added **N2 probability detection** for intelligent wake decisions.
- Added **smart wake alarm functionality** based on consecutive N2 detection.
- Added real-time communication between the **ESP32, backend, and frontend**.
- Added **FastAPI backend** for data processing and inference.
- Added **MQTT and WebSocket communication** for real-time data flow.
- Added **Redis** for real-time state management.
- Added **PostgreSQL + TimescaleDB** for persistent data storage.
- Added **React-based live dashboard** with sleep-stage visualization, HRV metrics, and alarm status.
- Added complete **frontend–backend integration and wiring**.
- Added an offline **machine learning training and evaluation pipeline**.
- Added **ONNX model export** and feature configuration.
- Added support for **SHHS, MESA, and ISRUC-Sleep** datasets in the ML pipeline.
- Added **Arduino IDE** and **PlatformIO** firmware workflows.
- Added Docker-based infrastructure for development and deployment.
- Added **mock ESP32 support** for testing without physical hardware.
- Established the modular project structure across **firmware, backend, ML, frontend, and infrastructure**.

## System Flow

**ECG Sensor → ESP32 → Signal Processing → RR Intervals → HRV Features → ML Inference → Sleep Stage Detection → Smart Wake → Live Dashboard**

The firmware implements the ECG-to-RR pipeline, while the backend performs feature processing, ML inference, and real-time dashboard communication.

## Core Technology Stack

| Layer | Technology |
|---|---|
| **ECG Sensor** | AD8232 |
| **Edge Device** | ESP32 |
| **Firmware** | Arduino / PlatformIO |
| **Sampling** | 250 Hz |
| **Backend** | FastAPI + Uvicorn |
| **Communication** | MQTT + WebSocket |
| **Machine Learning** | XGBoost + ONNX Runtime |
| **HRV Analysis** | hrv-analysis + NeuroKit2 |
| **State Management** | Redis |
| **Database** | PostgreSQL + TimescaleDB |
| **Frontend** | React + Vite + TailwindCSS |
| **Deployment** | Docker Compose |

## Contributors

- **David Immanuel Gobson** — Hardware / Firmware
- **Madhumanoj A** — Hardware
- **B Praveen** — ML / Backend / Frontend
- **Hariharasudhan A** — Frontend, Backend & Frontend–Backend Integration / Wiring

## Release Assets
//

## What's Changed
**Full Changelog:** `v1.0.0`

* Add introductory message to Readme.md by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/1
* Fix typo in README by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/2
* Update print statement from 'Hello' to 'Goodbye' by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/3
* guide.md  by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/4
* Delete .skills directory by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/5
* Create Firmware.md by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/7
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/8
* Add smart EEG alarm functionality by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/6
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/10
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/11
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/12
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/13
* Add initial HTML structure for frontend by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/14
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/15
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/16
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/17
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/18
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/19
* Add files via upload by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/20
* Upstream by @hariharasudhan-29507 in https://github.com/GobsonJR/SOMNUS-AI/pull/22

## New Contributors
* @hariharasudhan-29507 made their first contribution in https://github.com/GobsonJR/SOMNUS-AI/pull/1

**Full Changelog**: https://github.com/GobsonJR/SOMNUS-AI/commits/v1.0.0

## License

Released under the **MIT License**.

## What's Changed
* sync fork by @hariharasudhan-29507 in https://github.com/hariharasudhan-29507/SOMNUS-AI/pull/1
* Add Docker Image CI workflow by @hariharasudhan-29507 in https://github.com/hariharasudhan-29507/SOMNUS-AI/pull/2
* Delete Aura directory by @hariharasudhan-29507 in https://github.com/hariharasudhan-29507/SOMNUS-AI/pull/4

## New Contributors
* @hariharasudhan-29507 made their first contribution in https://github.com/hariharasudhan-29507/SOMNUS-AI/pull/1

**Full Changelog**: https://github.com/hariharasudhan-29507/SOMNUS-AI/commits/v1.0.0
