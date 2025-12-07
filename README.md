# TI MSPM0 Pro Micro

![License](https://img.shields.io/badge/License-CERN--OHL--W_v2-blue)
![Status](https://img.shields.io/badge/Status-Prototyping-yellow)
![KiCad](https://img.shields.io/badge/Designed_in-KiCad_8.0-white?logo=kicad)

A robust, drop-in replacement for the classic Pro Micro, powered by the **Texas Instruments MSPM0** series (Arm Cortex-M0+). This board modernizes the form factor with **USB Type-C** and **castellated edges** for easy surface mounting.

## 📷 Board Preview
*(Add a 3D render or photo of your board here)*
## ✨ Features

* **MCU:** TI MSPM0 Series (Arm Cortex-M0+)
    * *High-performance analog integration and low power consumption.*
* **Form Factor:** Classic Pro Micro Footprint
    * *Compatible with existing Pro Micro shields and keyboards.*
* **Connectivity:** USB Type-C
    * *Replaces the fragile Micro-USB connector.*
* **Mounting:** Castellated Edges (Half-holes)
    * *Allows the board to be soldered flat onto a carrier PCB (SMT assembly).*
* **User IO:** * *Standard Pro Micro pinout mapping.*
    * *Onboard LED indicators.*

## 🛠️ Technical Specifications

| Feature             | Details                                     |
| :------------------ | :------------------------------------------ |
| **Microcontroller** | TI MSPM0 (Specify: MSPM0G3507 / MSPM0L1306) |
| **Voltage**         | 3.3V Logic                                  |
| **Connector**       | USB Type-C (2.0 Data)                       |
| **PCB Specs**       | 2-Layer, 1.6mm thickness                    |
| **Dimensions**      | 18mm x 33mm (Approx)                        |

## 🚀 Design Process

This project was designed using **KiCad**. The layout process focused on signal integrity and manufacturability:

1.  **Schematic Capture:** Mapping the MSPM0 GPIOs to match the Pro Micro legacy pinout.
2.  **USB-C Implementation:** Robust routing for USB data lines (D+/D-) with impedance matching.
3.  **Layout Strategy:** * Optimized placement for decoupling capacitors near the MCU.
    * Careful routing of the Crystal/ROSC for clock stability.
    * Polygon pours for solid Power and Ground planes.
4.  **Fabrication Prep:** Designed with JLCPCB design rules in mind (DRC passed).

## 📦 Manufacturing

The Gerber files are generated for standard manufacturing processes.

* **Recommended Fab House:** JLCPCB (or similar).
* **Solder Mask:** Purple (or your choice).
* **Surface Finish:** ENIG (Recommended for flat castellations).

To order:
1.  Go to the `outputs/gerbers` folder.
2.  Upload the `.zip` file to the manufacturer website.

## 📄 License

**Hardware (Schematics/PCB):** [CERN-OHL-W v2](LICENSE)
**Documentation:** CC BY-SA 4.0

---
*Designed by [Sohel Ahmed Joni/JonyBepary].*
