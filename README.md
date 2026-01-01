# ESP32-C3 - Bare Bones DevKitM - KiCAD Source Files
---
This repo comes with a tutorial.

* [Save Battery Life on Your ESP32 - How to Make a custom PCB](https://bj-dehaan-solutions.com.au/articles/arduino-esp32-iot/save-battery-life-on-your-esp32-how-to-make-a-custom-pcb)
---
[![Project Available on PCBWay](pcb-project-image.png)](https://www.pcbway.com/project/shareproject/ESP32_C3_Bare_Bones_DevKitM_Ultra_Low_Power_ff5d294b.html)

![Assembled Board](esp32-c3-bare-bones-assembled.jpg)

## Goal: 

Create a simplified custom PCB based on the [ESP32-C3-DevKitM-1](https://docs.espressif.com/projects/esp-dev-kits/en/latest/esp32c3/esp32-c3-devkitm-1/user_guide.html)

This board is designed to consume as little power as possible while in deep sleep. Ideally 5uF as per the ESP-32 [datasheet](https://www.espressif.com/sites/default/files/documentation/esp32-c3-mini-1_datasheet_en.pdf). To this end the Voltage Regulator, RGB LED, Power LED and USB-UART interface have been removed. Leaving just the MCU, Reset/Boot button and header pins.

The board will need to be powered directly with a power source between 3.0 and 3.6v. It is important that the voltage never exceed 3.6v. Regular Lipo batteries typically have a maximum voltage of 4.2v so are not suitable.

This board was designed to be powered by a 3.2v LiFePO4 battery. Ideally charged with an external Battery Management System (BMS) that has a high-voltage cutoff at or below 3.6V. You can always test the batteries voltage first. If over 3.6V wait for it to discharge or apply small load with an LED for a few minutes.

The board will need to be programmed with an FDTI programmer as there is no USB interface.

[![Project Available on PCBWay](pcb-project-image.png)](https://www.pcbway.com/project/shareproject/ESP32_C3_Bare_Bones_DevKitM_Ultra_Low_Power_ff5d294b.html)

## Resources:

* [Save Battery Life on Your ESP32 - How to Make a custom PCB - Tutorial](https://bj-dehaan-solutions.com.au/articles/arduino-esp32-iot/save-battery-life-on-your-esp32-how-to-make-a-custom-pcb)
* [ESP32-C3-MINI-1 MCU Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32-c3-mini-1_datasheet_en.pdf)
* [ESP32-C3-DevKitM-1 Docs](https://docs.espressif.com/projects/esp-dev-kits/en/latest/esp32c3/esp32-c3-devkitm-1/user_guide.html)
* [ESP32-C3-DevKitM-1 Schematic](https://dl.espressif.com/dl/schematics/SCH_ESP32-C3-DEVKITM-1_V1_20200915A.pdf)


## Schematic:

[PDF Version](esp32-c3-bare-bones-schematic.pdf)

![Board schematic](esp32-c3-bare-bones-schematic.png)

## PCB Layout:

![Board schematic](esp32-c3-bare-bones-PCB.svg)