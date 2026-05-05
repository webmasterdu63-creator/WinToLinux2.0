<p align="center">
  <img src="assets/image.png" width="100%">
</p>
# WinToLinux 2.0  
### Install Linux from Windows — no USB, no ISO, no complexity.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
![Platform](https://img.shields.io/badge/Platform-Windows%2010%2F11-blue)
![Status](https://img.shields.io/badge/Status-Active-success)
![Web App](https://img.shields.io/badge/Web%20App-Online-brightgreen)
![Dual Boot](https://img.shields.io/badge/Dual--Boot-Supported-orange)
![Auto Update](https://img.shields.io/badge/Auto--Updating-Web%20Catalog-purple)

---

## 🚀 What is WinToLinux 2.0 ?

**WinToLinux 2.0 is a next‑generation Linux installer for Windows.**  
It combines a **modern Web App** (hosted on technews365.fr) with a **lightweight Windows Agent** to offer the simplest Linux installation experience ever created.

Inspired by **WSL2**, **ChromeOS Recovery**, and **GNOME Boxes**, but designed to install a **real Linux system** on your machine — with **dual‑boot**, **auto‑partitioning**, and **zero USB required**.

---

## ✨ Key Features

### 🔹 Install Linux without USB  
No more flashing tools, no more ISO juggling.  
Everything is downloaded and prepared automatically.

### 🔹 Automatic ISO detection  
The Web App fetches the latest:  
- LTS versions  
- Stable releases  
- New distributions  
- TechNews365 OS Ultimate builds  

### 🔹 Dual‑boot “Install alongside Windows”  
Automatic:  
- NTFS shrink  
- ext4 partition creation  
- bootloader configuration  
- UEFI support  

### 🔹 Full Install (Erase disk)  
For users who want a clean Linux‑only system.

### 🔹 USB Persistent Mode  
Create a persistent Linux USB directly from Windows.

### 🔹 Auto‑install via JSON profile  
The Web App generates an `install-profile.json` containing:  
- distro  
- ISO URL  
- checksum  
- install mode  
- language  
- timezone  
- disk layout  

The Windows Agent executes it automatically.

### 🔹 Cloud‑powered distro catalog  
Hosted on **technews365.fr**, always up to date.
WinToLinux 2.0 — Architecture

┌──────────────────────────────────────────────┐
│            WinToLinux Web App                │
│     (technews365.fr / Web Installer)         │
│                                              │
│  • Select distribution                        │
│  • Choose install mode                        │
│  • Generate install-profile.json              │
│  • Provide ISO metadata (LTS, Stable, etc.)   │
└───────────────────────────────┬──────────────┘
                                │
                                ▼
                 install-profile.json
                                │
                                ▼
┌──────────────────────────────────────────────┐
│              WinToLinux Agent (Windows)       │
│                                              │
│  • Reads install-profile.json                 │
│  • Downloads ISO                              │
│  • Verifies checksum                          │
│  • Shrinks NTFS (if alongside)                │
│  • Creates Linux partition                    │
│  • Prepares UEFI boot entry                   │
│  • Reboots into Linux installer               │
└───────────────────────────────┬──────────────┘
                                │
                                ▼
┌──────────────────────────────────────────────┐
│           TechNews365 / Linux Installer       │
│                                              │
│  • Auto-install using profile                 │
│  • Configure system                           │
│  • Install bootloader                         │
│  • Finalize dual-boot                         │
└──────────────────────────────────────────────┘




---

## 📦 Supported Distributions

- **TechNews365 OS Ultimate** (recommended)
- LMDE 7
- Debian 13
- Ubuntu 24.04 LTS
- Linux Mint 22
- Zorin OS 17
- Fedora Workstation
- KDE Neon
- Pop!_OS
- And more…

---

## 🛠 Project Structure

wintolinux/
│
├── web/                # Web App (HTML/CSS/JS/PHP)
│   ├── api/            # distros.json, metadata
│   ├── ui/             # pages, components
│   └── assets/         # icons, css, branding
│
├── agent/              # Windows executable source
│   ├── downloader/     # ISO download + checksum
│   ├── partitioner/    # NTFS shrink + ext4 creation
│   ├── bootloader/     # UEFI entry creation
│   └── installer/      # profile interpreter
│
├── docs/               # documentation, diagrams
│
└── LICENSE             # GPLv3
Code


---

## 📄 License

WinToLinux 2.0 is released under the **GNU GPLv3** license.  
See the `LICENSE` file for details.

---

## 🌐 Official Website

**https://technews365.fr/wintolinux**

---

## 🤝 Contributing

Contributions are welcome!  
Pull requests, issues, and feature suggestions are encouraged.

---

## ⭐ Support the Project

If you like WinToLinux 2.0, give the repo a **star** ⭐  
It helps visibility and supports future development.

---

## 🧩 Architecture Overview

