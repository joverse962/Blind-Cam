<div align="center">

# 👁️‍🗨️ Blind-Cam
### v1.0 PROTOTYPE - ESP-CSI VISUALIZER

![Status](https://img.shields.io/badge/Status-Prototype-orange?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-ESP32_C3-blue?style=flat-square)
![Tech](https://img.shields.io/badge/Tech-CSI_Spectroscopy-purple?style=flat-square)
![Lang](https://img.shields.io/badge/Language-C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)

[🌐 **Visit Project Website**](https://joverse.netlify.app/blind-cam/)

---

### 📡 A handheld scope for the invisible world.
**Real-time Wi-Fi Channel State Information (CSI) visualization.**

[Concept](#-the-vision) • [Hardware](#-hardware-manifest) • [Firmware](#-software--firmware) • [Modes](#-visual-modes)

<img src="https://github.com/Abdullah-Alawad/imgs/blob/main/hero1.png?raw=true" alt="Blind-Cam Hero View" width="80%">
</div>

---

## 🔭 The Vision

### The "Blind" Concept
We are swimming in a sea of Wi-Fi signals that bounce off walls, furniture, and bodies. Most devices discard this reflection data as "noise," but Blind-Cam captures and analyzes it to render the environment.

> **🧠 Philosophy:** "Cameras capture light; the Blind-Cam captures data."

**Current Capabilities:**
* 🕵️ **Sniffer Mode:** Passive traffic monitoring and packet capture.
* 📈 **Live Viz:** Smooth 60FPS TFT rendering of spectral data.
* 🔋 **Portable:** Fully self-contained unit with internal LiPo power.

---

## 🧰 Hardware Manifest

A low-cost, high-availability Bill of Materials designed for rapid replication.

| Component | Description | Preview |
| :--- | :--- | :---: |
| **ESP32-C3 Mini** | 🧠 **The Brain.** RISC-V single-core MCU handling high-frequency CSI packet sniffing. | <img src="https://github.com/Abdullah-Alawad/imgs/blob/main/esp32.png?raw=true" width="80"> |
| **1.8" TFT Display** | 📺 **The Eyes.** SPI Interface screen for real-time spectral rendering and histograms. | <img src="https://github.com/Abdullah-Alawad/imgs/blob/main/tft.png?raw=true" width="80"> |
| **LiPo Power** | ⚡ **The Fuel.** Internal rechargeable power source for true cordless field analysis. | <img src="https://github.com/Abdullah-Alawad/imgs/blob/main/battery.png?raw=true" width="80"> |

---

## 💻 Software & Firmware

The core logic is written entirely in **C++** to ensure maximum performance on limited hardware resources.

* **⚡ Optimized C++ Kernel:** Custom packet-handling routines designed to strip CSI headers with zero-copy overhead.
* **🔢 Edge Computing:** All signal processing (FFT and noise filtering) happens locally on the ESP32—no cloud connection required.

---

## 🏗️ Fabrication / Modular Housing

The unit features a custom **Modular Housing Design** fabricated via FDM 3D printing. The chassis is split into two distinct functional modules (Body & Cover) to allow for easy maintenance and battery hot-swapping.

<div align="center">
  <img src="https://github.com/Abdullah-Alawad/imgs/blob/main/prusa3.jpg?raw=true" width="60%" style="border-radius: 10px;">
  <p><i>🖨️ Fabricated on Prusa XL - Rapid Prototyping</i></p>
</div>

### ⚙️ Housing Details
Designed with tight tolerances to friction-fit the display without screws, keeping the center of gravity low for maximum stability during handheld use.

<div align="center">
  <img src="https://github.com/Abdullah-Alawad/imgs/blob/main/pic3.jpg?raw=true" width="40%" style="border-radius: 10px; margin: 5px;">&nbsp;&nbsp;
  <img src="https://github.com/Abdullah-Alawad/imgs/blob/main/pic4.jpg?raw=true" width="40%" style="border-radius: 10px; margin: 5px;">
</div>

---

## 📊 Visual Modes

The software interprets raw CSI data in distinct ways to visualize the invisible electromagnetic environment.

### 1️⃣ Waterfall Plot (Heatmap)
Historical heat map allowing users to see movement patterns and signal changes over time.
<div align="center">
<img src="https://github.com/Abdullah-Alawad/imgs/blob/main/pic5.jpg?raw=true" width="50%" style="border-radius: 10px;">
</div>

<br>

### 2️⃣ Spectral View & Statistics
Real-time frequency domain representation (**Left**) and Signal Intensity/Noise Floor monitoring (**Right**).
<div align="center">
  <img src="https://github.com/Abdullah-Alawad/imgs/blob/main/pic2.jpg?raw=true" width="40%" style="border-radius: 10px; margin: 5px;">&nbsp;&nbsp;
  <img src="https://github.com/Abdullah-Alawad/imgs/blob/main/pic1.jpg?raw=true" width="40%" style="border-radius: 10px; margin: 5px;">
</div>

---

<div align="center">

✨ **JOVERSE** © 2025 ✨
*Rendering the Invisible.*

</div>
