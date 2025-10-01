# BAD-USB

## ⚠️ Caution 

For educational and authorized security‑testing purposes only. Do not use this project to compromise systems without explicit permission.


---

## Table of Contents
- [Project Overview](#project-overview)  
- [Key Features](#key-features)  
- [Use Cases](#use-cases)  
- [Hardware & Software Requirements](#hardware--software-requirements)  
- [Quick Install (Build & Flash)](#quick-install-build--flash)  
- [Usage Examples](#usage-examples)  
- [Payload Development](#payload-development)  
- [Security, Ethics & Legal](#security-ethics--legal)  
- [Contributing](#contributing)  
- [Roadmap](#roadmap)  
- [License & Credits](#license--credits)  
- [Contact](#contact)

---

## 💻 About the Project

EvilDuck is an open‑source hardware and software platform that implements HID (Human Interface Device) keyboard emulation to execute preconfigured payloads on host systems. Engineered as a low‑cost, fully customizable alternative to commercial tools (e.g., USB Rubber Ducky), the project leverages widely available microcontrollers and components to deliver repeatable, scriptable keystroke attacks for red‑team assessments, device hardening tests, and research. Designed for use in authorized security testing, EvilDuck provides a compact, extensible framework for developing and validating automated input‑based attack scenarios and mitigations.
Antes de começar, verifique se você atendeu aos seguintes requisitos:



## Project Overview
BAD‑USB is an open‑source hardware and firmware platform that implements USB HID (Human Interface Device) keyboard emulation to execute scripted input sequences on target hosts. Designed as a low‑cost, extensible alternative to commercial keystroke injectors, the project collects board references, PCB resources, firmware examples, and payload templates for controlled laboratory use.

This repository is intended for security engineers, researchers, and educators to evaluate endpoint resilience to automated input attacks, develop mitigations, and create repeatable test cases for red/blue team exercises.

---

## Key Features
- Emulates USB keyboard devices to execute scripted payloads.  
- Firmware examples compatible with commonly available microcontrollers.  
- Payload templates and builder conventions for repeatable tests.  
- Hardware reference files (schematics, PCB layouts) for low‑cost builds.  
- Extensible architecture to add new modules and host interactions.

---

## Use Cases
- Authorized red team proof‑of‑concepts and security assessments.  
- Endpoint hardening validation (HID controls, endpoint detection).  
- Educational labs on USB, firmware development, and payload scripting.  
- Research into detection and mitigation of automated input attacks.

---

## Hardware & Software Requirements

### Recommended hardware
- Microcontroller with native USB HID support (e.g., ATmega32U4-based boards such as Pro Micro, Arduino Micro, or equivalent).  
- Optional: SD card / filesystem for payload storage.  
- Basic PCB and enclosure components (see `hardware/` directory).

### Toolchain / software
- Arduino IDE or PlatformIO for compiling and flashing firmware.  
- avrdude or vendor flashing tools for your MCU.  
- Python 3.x (optional) for payload builder scripts and helpers.  
- Git for source control.

---

## Quick Install (Build & Flash)

> Adapt the commands below to your selected MCU and flashing tool.

1. Clone the repository:
```bash
git clone https://github.com/nassim-saii/BAD-USB.git
cd BAD-USB
