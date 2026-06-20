# DevBoard

Custom RP2040-based development board for embedded systems and hardware prototyping.

## Images

### Front
![Front](image/front.png)
<img width="1512" height="947" alt="Screenshot 2026-06-02 at 10 48 57 AM" src="https://github.com/user-attachments/assets/7f0fe45c-6121-4fc0-b69f-15a6effe49f1" />


### Back
![Back](image/back.png)

### PCB
![PCB](image/pcb.png)

### Schematic
![Schematic](image/schema.png)

---


## Bill of Materials (BOM)

The following BOM was used for the RP2040 DevBoard.

| Ref | Qty | Component | LCSC Part # | Manufacturer Part # |
|------|-----:|------------|------------|------------|
| C1, C10 | 2 | 1uF 0402 Capacitor | C52923 | CL05A105KA5NQNC |
| C2-C12, C17 | 11 | 100nF 0402 Capacitor | C1525 | CL05B104KO5NNNC |
| C13, C14 | 2 | 10uF Capacitor | C19702 | CL10A106KP8NNNC |
| C15, C16 | 2 | 15pF 0402 Capacitor | C1548 | 0402CG150J500NT |
| D2 | 1 | SK6812MINI-E RGB LED | C5149201 | SK6812MINI-E |
| J1 | 1 | USB Type-C Connector | C165948 | TYPE-C-31-M-12 |
| R1, R2 | 2 | 5.1kΩ 0402 Resistor | C25905 | 0402WGF5101TCE |
| R3, R5 | 2 | 1kΩ 0402 Resistor | C11702 | 0402WGF1001TCE |
| R4 | 1 | 10kΩ 0402 Resistor | C25744 | 0402WGF1002TCE |
| R6, R7 | 2 | 27Ω 0402 Resistor | C25100 | 0402WGF270JTCE |
| SW1 | 1 | Push Button | C720477 | TS-1088-AR02016 |
| U1 | 1 | RP2040 Microcontroller | C2040 | RP2040 |
| U2 | 1 | MCP1700 3.3V LDO | C39051 | MCP1700T-3302E/TT |
| U3 | 1 | W25Q16JVUXIQ SPI Flash | C2843335 | W25Q16JVUXIQ |
| Y1 | 1 | 12MHz Crystal | C9002 | X322512MSB4SI |

### Notes

- Designed around the Raspberry Pi RP2040 microcontroller.
- Uses a 12MHz external crystal and Winbond SPI flash.
- USB Type-C connector footprint is compatible with HRO TYPE-C-31-M-12.
- All resistors and capacitors use 0402 footprints unless otherwise noted.
- Some LCSC parts may become unavailable over time; equivalent parts with matching value, package, and electrical specifications may be substituted.
- For the latest sourcing information, see [`bom/bom.csv`](bom/bom.csv).

### Estimated Cost

| Item | Approx. Cost (USD) |
|--------|--------:|
| RP2040 | $1.00 |
| Flash Memory | $2.40 |
| USB-C Connector | $0.19 |
| Crystal | $0.10 |
| LDO Regulator | $0.46 |
| RGB LED | $0.09 |
| Passives + Switch | ~$1.00 |
| **Total Electronics Cost** | **~$5–6 per board** |

> Prices vary depending on supplier stock and order quantity.



## Features

- RP2040 Microcontroller
- USB Support
- GPIO Breakout
- I2C / SPI / UART
- Custom PCB Design

---

## Repository Structure

```text
devboard/
│
├── grb/
├── image/
├── kicad/
├── grb.zip
└── README.md
```

---

## Files

- `grb/` → Gerber manufacturing files
- `image/` → Board images and schematic
- `kicad/` → KiCad design files
- `grb.zip` → Exported Gerber archive

---

## Author

Created by [AYUSH-pro-grammer](https://github.com/AYUSH-pro-grammer)
