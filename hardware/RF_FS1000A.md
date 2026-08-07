# FS1000A RF module for Lilka

Based on https://github.com/BruceDevices/firmware/wiki/RF#unofficial-modules not yet tested

## Compatibility
Bruce firmware, limited to ASK/OOK modulation. Might not work well with 3.3v supply

## Inventory
- 4-pin 433 Mhz Wireless Receiver Module (often sold with FS1000A)
- 20x80 prototype PCB
- female 12-pin header
- thin copper wires
- a ceramic capacitor 0.2-0.5uF (optional)

## Wiring (TODO)
| Lilka J2 # | Lilka pin | LoRa pin |
|------------|-----------|----------|
| 1          | GND       | GND      |
| 2          | 3V3       | VCC      |
| 3          | RX (44)   |     |
| 4          | TX (43)   |     |
| 5          | 48        |     |
| 6          | 47        |     |
| 7          | 21        |     |
| 8          | 14        |     |
| 9          | 13        |     |
| 10         | 12        |     |
| 11         | 3V3       |          |
| 12         | GND       |          |

