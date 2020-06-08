# DFU Mode

## Purpose
Arduino Uno has a chip to connect between USB port and Arduino main chip (Atmega328p). That chip has a firmware to be a USB-to-serial (Arduino-usbserial), but we can charge to different type of USB driver by entry DFU mode and application.

*   USB driver:
    -   MIDI controller
    -   HID driver
        +   Keyboard
        +   Mouse
        +   Joystick

## Usage
*   Setup:
    -   Windows: FLIP
    -   MAC & Linux: dfu-programmer
*   Arduino
    -   Atmega8u2/16u2
    -   ...

## Arduino
Connect the RESET and GND pin together to disconnect the COM and LPT with PC. At this moment, arduino (atmega8u2/16u2) is waiting and ready to programming.

![](images/image_thumb[16].png)

## Install
### Windows
Download [Atmel FLIP](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/FLIP) and install to path "C:\Program Files\Atmel\Flip 3.4.5\usb". Once the installer finished, the driver will be detect as USB-Win32 Devices, which is meaning the FLIP already install successfully.

### Linux
You can follow the [link](https://www.arduino.cc/en/Hacking/DFUProgramming8U2) to install dfu-programmer. OR, use a command line as show bottom:
```bash
> sudo apt-get install dfu-programmer
```
OR
```bash
> sudo aptitude install dfu-programmer
```