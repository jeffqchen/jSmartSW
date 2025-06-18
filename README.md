![image](https://github.com/user-attachments/assets/b72ef1bd-7279-4c3d-9a03-44363c54772e)

A smart controller for gScartSW v5.2 that works with RetroTink 4K. This device connects to the gSCARTsw v5.2 via the unpopulated 8-pin EXT port and enhances the gSCARTsw on multiple aspects.

# Main Features

- Automatically switch profiles on the RetroTink 4K with input changes on the gSCARTsw
- Control which input is active on the gSCARTsw, beside using it's orignal auto input detection.
- See which input is selected on the gSCARTsw from the OLED screen or RGB LEDs.
- Power the gSCARTsw with a barrel jack or USB-C, with an actual power switch that can turn power off.
- Control RetroTink 4K with various USB controllers, or even a keyboard/mouse.

Please refer to Project Wiki pages for more detailed information.

# Quick User Reference Guide

## Hardware

### Main Board

![image](https://github.com/user-attachments/assets/9b3c9766-7b6a-420e-9871-22fa038c6d9f)

### Keypad

![image](https://github.com/user-attachments/assets/26aee5cb-a52c-41d6-9f97-2cac8b780683)


## Functionality

### Main Board

The main functionality of the main board is to notify the RetroTink 4K of the change and trigger an SVS profile change via serial commands when the selected input on the gSCARTsw changes. This is a hard-coded automated process and does not require user interference.

Please refer to the [RetroTink 4K Wiki](https://consolemods.org/wiki/AV:RetroTINK-4K#Load_Profile) for details on how to set up the SVS profiles.

### Keypad

![image](https://github.com/user-attachments/assets/969b370a-b35e-42d5-88aa-44e53472b07e)

The keypad has 8 keys, corresponding to each of the inputs on a gSCARTsw. An OLED screen and 16 addressable RGB LEDs provide visual feedback of the operation state.

A firm press on a key will trigger a corresponding input change, as well as notifying the RetroTink 4K with an SVS profile change command.

If `1/SHIFT` is held, you can use the various functions marked below each of the input keys.

Holding an input key for longer than 2 seconds will trigger input icon customization. You will be able to choose an icon for the corresponding input for better recognition.

### USB Input Devices

![image](https://github.com/user-attachments/assets/bc277d80-6a3d-404e-b406-9c16c191ae33)

You can connect various USB HID devices to operate the jSmartSW. Supported USB devices include:

Sony:
- DualShock 3
- DualShock 4
- DualSense
- [PSX2USB](https://github.com/jeffqchen/PSX2USB_hardware)


Nintendo
- Switch JoyCon Charging Grip
- Switch Pro Controller
- 8bitdo M30 2.4g (Pro Controller Mode)

Sega
- Saturn USB Controller
- [Genesis 2X Controller to USB Adapter](https://github.com/jeffqchen/Genesis-2X-Controller-to-USB-Adapter)

Generic
- USB Keyboard
- USB Mouse

