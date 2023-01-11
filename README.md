# PicaChoc36

Low-profile split keyboard with 36 keys using XIAO controllers.

_Pica pica - european (common) magpie_

<img src='images\main.jpg' width="600">

## Features

- reversible PCB
- 36 soldered ChocV1 keys
- wired/wireless versions
- top pinky key moved to side
- 3D printed case

### Wired version

- XIAO RP 2040 controller
- QMK firmware
- TRRS or USB-C connection between halves
- rotary encoder on one side
- one status LED

### Wireless version

- XIAO BLE controller
- _[TODO]_ ZMK firmware
- rotary encoder on both sides (ZMK supports only main side for now)
- on/off toggle
- battery connectors

## Photos

wired version with 3d printed case

<img src='images\top.jpg' width="600">
<img src='images\side.jpg' width="600">
<img src='images\bottom.jpg' width="600">

battery compartment

<img src='images\battery.jpg' width="600">

## Firmware

- QMK - [my fork](https://github.com/zzeneg/qmk_firmware/tree/feature/picachoc36/keyboards/picachoc36), [compiled file](firmware/qmk/picachoc36_rev1_default.uf2).
- Vial - [my fork](https://github.com/zzeneg/vial-qmk/tree/feature/picachoc36/keyboards/picachoc36), [compiled file](firmware/vial/picachoc36_rev1_vial-zzeneg.uf2) and [vial config](firmware/vial/zzeneg.vil).
- _[TODO]_ ZMK

## Gerber files

- [PCB](gerbers/pcb.zip)

## Case files (STL - 3d printed)

- Wired - [Left](stl/Plate-wired-left.stl), [left without encoder hole](stl/Plate-wired-left-noenc.stl), [right](stl/Plate-wired-right.stl), [right without encoder hole](stl/Plate-wired-right-noenc.stl)
- Wireless - with battery compartment and encoder holes - [left](stl/Plate-wireless-left.stl), [right](stl/Plate-wireless-right.stl)

## Bill of materials

- PCBs
- 3D printed case
- 2 XIAO MCUs - [RP2040](https://www.seeedstudio.com/XIAO-RP2040-v1-0-p-5026.html) for wired version, [nRF52840](https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html) for wireless
- 36 Choc V2 switches
- 36 SMD SOD-123 1N4148 diodes
- 1 or 2 EC11/12 rotary encoder with knob, [low profile](https://keycapsss.com/keyboard-parts/parts/220/alps-alpine-encoder-low-profile-ec12e1220301) is recommended
- _[Wired only]_ [2x USB-C 16pin connector](https://www.aliexpress.com/item/1005003670899595.html) or TRRS jack
- _[Wired only]_ USB-C or TRRS cable
- _[Wireless only]_ 2x Li-Ion 3.7V battery (battery compartment suited for 5×12×21 size)
- _[Wireless only]_ [2x on/off toggle MSK-12C02](https://www.aliexpress.com/item/4000685483225.html)

## Build log

**TODO**

Similar to all other keyboards.

Diodes are soldered on top side.

⚠️ Flash your MCUs with a firmware that supports bootmagic/QK_BOOT/&reset functions, and triple check all keys with tweezers before soldering switches, it's not possible to disassemble the keyboard without desoldering.
