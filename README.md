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

### 🔹 Lightweight Windows Agent  
Handles:  
- ISO download  
- checksum verification  
- partitioning  
- bootloader setup  
- reboot into installer  

---

## 🧩 Architecture Overview

