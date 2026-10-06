# 1TX/2RX FMCW Radar System

![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-in%20development-blue.svg)

A comprehensive hardware and software implementation of a **Frequency Modulated Continuous Wave (FMCW) Radar** system featuring 1 Transmitter (TX) and 2 Receivers (2RX) utilizing the **ADALM-PLUTO** SDR, controlled via a **NEMA 23 stepper motor** positioning platform.

---

## 🚀 System Overview

This project is designed to bridge RF engineering, digital signal processing (DSP), and embedded motion control. The system sweeps frequencies to transmit continuous waves, captures reflections through dual receiver channels, and processes range-Doppler maps while mechanically scanning the environment via a precision stepper motor.

### Key Features:
* **SDR Integration:** ADALM-PLUTO configured for 1TX / 2RX multi-channel coherent operation.
* **Mechanical Scanning:** NEMA 23 stepper motor driving a custom rotating platform for azimuth/elevation sweeps.
* **Signal Processing:** Range-Doppler estimation, Fast Fourier Transform (FFT) filtering, and target detection algorithms.
* **Modular Architecture:** Clean separation between mechanical designs, hardware schematics, and DSP software.

---

## 📂 Repository Structure

fmcw-radar-system/
├── hardware/
│   ├── mechanics/          # 3D printable chassis, rotating platform, and STEP/STL files
│   └── electronics/        # NEMA 23 driver schematics, power distribution, and wiring diagrams
├── software/
│   ├── sdr_processing/     # Python / MATLAB scripts for ADALM-PLUTO signal acquisition & DSP
│   └── motor_control/      # Stepper motor driver firmware / control scripts
├── docs/                   # System architecture diagrams, datasheets, and test results
└── README.md

---

## 🛠️ Hardware & Components

* **SDR:** Analog Devices ADALM-PLUTO (Custom firmware/config for 2RX sync)
* **Actuator:** NEMA 23 Stepper Motor paired with a high-torque driver
* **Antennas:** Directional patch/horn antennas optimized for the target frequency band
* **Processing Unit:** PC running Python / MATLAB / GNU Radio

---

📜 License
This project is open-source and licensed under the MIT License.

```text