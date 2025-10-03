# BAD-USB

## ⚠️ Caution 

For educational and authorized security‑testing purposes only. Do not use this project to compromise systems without explicit permission.

---

## Overview
BAD‑USB is an open‑source hardware and firmware project demonstrating USB HID (Human Interface Device) keyboard emulation to execute scripted input sequences on host systems. This repository includes firmware examples, payload templates, and hardware references intended for controlled laboratory use to support USB hardening assessments, red‑team/blue‑team exercises, and security research.

---


<div align="center"> 
  <img src="https://github.com/nassim-saii/BAD-USB/blob/main/Pic1.jpg" alt="screenshot" width="Auto" height="Auto" />
</div>
<div align="center">
  <img src="https://github.com/nassim-saii/BAD-USB/blob/main/PICs/F-Back%20View.png"  width="300"/>
  <img src="https://github.com/nassim-saii/BAD-USB/blob/main/PICs/F-Front%20%20View.png"  width="300"/> 
</div>

---



## Repository structure (high level)
- `BAD-USB_Code/` — Arduino/MCU sketches (`.ino`) and build notes.  
- `scripts/` — example payload text files (e.g., `script.txt`).  
- `PCB/` — schematics, PCB artwork, and reference images.  



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
```

## Common directives

- `DELAY/` <ms> — wait <ms> milliseconds.
- `STRING/` <text> — type <text> as keyboard input.
- `ENTER/` — press Enter/Return.
- `TAB/` — press Tab.
- `ESC/` — press Escape.
- `CTRL/`, `ALT/`, `SHIFT/` — used in combination or on their own depending on parser implementation.
- `REPEAT/` <n> — repeat previous command <n> times (if implemented).



## Responsible testing & legal

By using this repository you agree to:
- **Obtain explicit, written authorization before testing systems you do not own.
- **Limit testing to isolated labs, VMs, or assets with owner consent.
- **Avoid destructive payloads or unauthorized exfiltration unless explicitly approved.
- **Comply with applicable laws and organizational policies.
  
The maintainers disclaim liability for misuse. Misuse of HID emulation devices can be illegal and cause serious harm.
