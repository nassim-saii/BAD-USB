# BAD-USB

## ⚠️ Caution 

For educational and authorized security‑testing purposes only. Do not use this project to compromise systems without explicit permission.



---

## Overview
BAD‑USB is an open‑source hardware and firmware project demonstrating USB HID (Human Interface Device) keyboard emulation to execute scripted input sequences on host systems. This repository includes firmware examples, payload templates, and hardware references intended for controlled laboratory use to support USB hardening assessments, red‑team/blue‑team exercises, and security research.

---

## Repository structure (high level)
- `firmware/` — Arduino/MCU sketches (`.ino`) and build notes.  
- `payloads/` or `scripts/` — example payload text files (e.g., `script.txt`).  
- `hardware/` or `PCB/` — schematics, PCB artwork, and reference images.  
- `docs/` — optional documentation, lab guides, and contributor notes.

> Verify exact folder names in the repository root and adapt paths as needed.

---

## Key features
- Emulates USB HID keyboards to execute scripted keystrokes.  
- Example `.ino` firmware compatible with ATmega32U4‑class boards (Pro Micro / Arduino Micro).  
- Plain‑text payload scripts using simple directives (`DELAY`, `STRING`, `ENTER`, etc.).  
- Hardware reference files for low‑cost prototype builds.  
- Designed for repeatable, auditable test cases in authorized environments.

---

## Quick start — environment preparation
1. Clone the repository:
```bash
git clone https://github.com/nassim-saii/BAD-USB.git
cd BAD-USB
