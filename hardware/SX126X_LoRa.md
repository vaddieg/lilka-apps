# SX126x LoRa module for Lilka

Following works with E22, DX-LR20, DX-LR30 and most likely other SPI LoRa modules.

## Compatibility
Meshtastic, Meshcore, Bruce LoRa chat

## Inventory
- LoRa module
- 20x80 prototype PCB
- female 12-pin header
- thin copper wires
- a ceramic capacitor 0.2-0.5uF (optional)

## Wiring
| Lilka J2 # | Lilka pin | LoRa pin |
|------------|-----------|----------|
| 1          | GND       | GND      |
| 2          | 3V3       | VCC      |
| 3          | RX (44)   | DIO1     |
| 4          | TX (43)   | BUSY     |
| 5          | 48        | NRST     |
| 6          | 47        | MISO     |
| 7          | 21        | MOSI     |
| 8          | 14        | SCK      |
| 9          | 13        | NSS      |
| 10         | 12        | RXEN     |
| 11         | 3V3       |          |
| 12         | GND       |          |

Additionally connect LoRa **TXEN** to LoRa **DIO2**. Optionally, solder the capacitor to GND and VCC lines next to the module.  
