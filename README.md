# My-Hackpad
# Custom 9-Key Mechanical Macro Pad

A custom input device featuring a 3x3 mechanical keyswitch grid, an incremental rotary encoder knob, and an OLED display screen. This project was built from scratch as part of the **Hack Club Stardance Hackpad Challenge**.

## 🛠️ Hardware Features
- **Microcontroller:** Seeed Studio XIAO 
- **Keyswitches:** 9 Mechanical MX style switches arranged in a 3x3 grid.
- **Rotary Encoder:** 1 encoder knob with an integrated push-button click switch.
- **Display:** I2C OLED screen for visual feedback and device status tracking.
- **Form Factor:** Compact layout optimized within required board dimension limits, featuring physical mounting holes for secure enclosure mounting.

---

## 💻 Project Contents

This repository contains all the design and manufacturing assets needed to build the device:
- **Schematic & PCB Design:** Complete KiCad project files containing the full electrical wiring layouts and footprints.
- **Fabrication Packages:** Production-ready Gerber and Drill files bundled together for direct manufacturing submission.
- **3D Case Modeling:** Enclosure and shell design files exported for 3D printing or assembly planning.
- **Firmware Profile Source:** Dedicated code files defining the component matrix pins, peripheral drivers, and initial key mapping functions.

---

## ⌨️ Matrix and Component Routing

The electronics utilize a multiplexed row and column matrix grid to efficiently read all physical switch inputs while preserving dedicated pins for the peripheral hardware buses:
- The 9 mechanical keys and the rotary encoder's push-button click switch are wired into intersecting matrix lines protected by anti-ghosting diodes.
- The rotary encoder rotation pins connect to dedicated digital lines to capture directional spinning actions.
- The OLED display handles data communication via the standard hardware I2C bus pins.
- All active devices run safely off the shared 3.3V power bus network.

---

## BOM

- 1 unsoldered Seeed XIAO RP2040
- 9x through-hole 1N4148 Diodes
- 9x MX-Style switches
- 1x EC11 Rotary encoders
- 1x 0.91 inch OLED display
- 9 white blank DSA keycaps
- 4x M3x16mm screws
- 4x 6x M3x5mx4mm heatset inserts

<img width="2266" height="1488" alt="IMG_0557" src="https://github.com/user-attachments/assets/d4fb6753-830e-4ab3-812f-ff85d950944b" />
<img width="2266" height="1488" alt="IMG_0558" src="https://github.com/user-attachments/assets/8999d44b-2e82-4ef4-8d40-e6a768420c0b" />
<img width="769" height="533" alt="Screenshot 2026-08-23 at 02 02 40" src="https://github.com/user-attachments/assets/6503feec-7ef5-4ab1-a8b0-2205d5490a01" />
<img width="1374" height="803" alt="Screenshot 2026-08-23 at 02 02 15" src="https://github.com/user-attachments/assets/451f4967-ace7-4a62-a7c5-e2588e1f66a9" />
