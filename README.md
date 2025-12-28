## R.E.V.E.N.G.E  
**Realy Expensive Vainglory Expirence Negating Genuine Ease**  

A line‑follower robot built for the Russian tech competition **robofinist.org**.

---  

### Overview  
- **Created:** 15 Nov 2025  
- **Based on:** [Differential robot](https://github.com/armv7-mmio/Differential)  
- **Development stack:** GNU/Linux, Vim, ARM GCC toolchain and Cmake, ST‑HAL libraries, FreeCAD  

---  

### Hardware  

| Component | Part / Description | Key Specs |
|-----------|-------------------|-----------|
| **MCU** | STM32F411CEU6 | Arm® Cortex®‑M4, 32‑bit, FPU |
| **Motors** | GA12‑N30 | 3 V, 1000 rpm |
| **Motor driver** | DRV8833 | Dual H‑bridge, 1.5 A per channel |
| **Distance sensor** | HC‑05 (Bluetooth) + VS1838 (IR) | On/off detection, telemetry |
| **Line sensors (×7)** | ITR8307 / S17 / TR8B (SMD) | Infrared reflectance |
| **Power** | LiPo 103048 | 3.7 V, 1500 mAh, PH‑2 connector |

---  

### Firmware  

- **Language:** C (ARM‑CMSIS/STM32 HAL)  
- **Build system:** Cmake with ARM GCC Toolchain  
- **Features:**  
  - Real‑time line‑tracking PID controller  
  - Bluetooth telemetry via HC‑05  
  - IR distance detection for obstacle avoidance  
  - Power‑management routines for LiPo safety  

*The firmware is currently under active development.*

---

### License  

This project is released under the **GPLv2**. See `LICENSE` for details.  
