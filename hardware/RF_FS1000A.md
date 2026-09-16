# FS1000A + XY-MK-5V RF module for Lilka

Based on https://github.com/BruceDevices/firmware/wiki/RF#unofficial-modules

## Compatibility
Bruce firmware, limited to legacy ASK/OOK modulation. 433 MHz Remote Control apps.
Bruce settings: RX 14,  TX 21

## Inventory
- 4-pin FS1000A 433 Mhz Wireless Receiver
- 3-pin XY-MK-5V 433 Mhz Wireless Transceiver 
- 2x 433 MHz helical antennas or 2x 16.5cm single-core copper wires
- 20x80 prototype PCB
- female 12-pin header
- thin copper wires
- a ceramic capacitor 0.2-0.5uF (optional)

## Wiring
| Lilka J2 # | Lilka pin | Module pin |
|------------|-----------|------------|
| 1          | GND       | GND      |
| 2          | 3V3       | VCC      |
| 3          | 44        |     |
| 4          | 43        |     |
| 5          | 48        |     |
| 6          | 47        |     |
| 7          | 21        |     |
| 8          | 14        |     |
| 9          | 13        |     |
| 10         | 12        |     |
| 11         | 3V3       |          |
| 12         | GND       |          |

## Status
Assembled and tested on a breadboard using Bruce. Decided not to solder a module due to limited usefulness 
