# MeshCore companion firmware for Lilka

## Compatibility
MeshCore firmware is compatible with Lilka SX126x radio modules. See the **hardware** directory.

## Official repository
https://github.com/meshcore-dev/MeshCore

## Lilka port
You can get sources from here:
https://github.com/ab4o1on/MeshCore

## Build instructions for MeshCore firmware

1. Clone the https://github.com/ab4o1on/MeshCore repository
2. Open the firmware project in VS Code and let Pioarduino to download the necessary dependencies
3. Press Ctrl-Shift-P (Command-Shift-P) and choose "Pick Project Environment"
4. Select "Lilka_sx1262_companion_radio_ble" (other device roles might work too) from the list
5. In Pioarduino select General->Build and wait for compilation to finish
6. Open the hidden *.pio/build/Lilka_sx1262_companion_radio_ble* subdirectory
7. Find the *firmware.bin* file
8. Copy the file to Lilka SD card
