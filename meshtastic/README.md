# Build instructions for Meshtastic firmware

1. Clone the https://github.com/meshtastic/firmware repository and check out a stable release
2. Copy **lilka** directory into Meshtastic's *variants/esp32s3/diy*
3. Open the firmware project in VS Code and let Pioarduino to download the necessary dependencies
4. Press Ctrl-Shift-P (Command-Shift-P) and choose "Pick Project Environment"
5. Select "lilka" from the list
6. In Pioarduino select General->Build and wait for compilation to finish
7. Open the hidden *.pio/build/lilka* subdirectory
8. Among the firmware bin files pick one without *factory* or *littlefs* in its name
9. Copy the file to Lilka SD card
