# SX126x LoRa module for Lilka

Following works with E22, DX-LR20, DX-LR30 and most likely other 12-pin SPI LoRa modules.
<img width="402" height="359" alt="Screenshot 2026-08-14 at 16 07 43" src="https://github.com/user-attachments/assets/a8635eec-7a21-4817-aab4-7783699bf82e" />


## Compatibility
Meshtastic, Meshcore, Bruce LoRa chat

## Inventory
- LoRa module
- 20x80 prototype PCB
- female 12-pin header
- thin copper wires
- a ceramic capacitor 0.2-0.5uF (optional)

  <img width="544" height="385" alt="components" src="https://github.com/user-attachments/assets/7269fe72-5b5b-48e5-96be-0f51c9175015" />


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

## Assembly
There are many intersecting wires, use both sides of PCB to lay them out. You can change the orientation of the 12-pin header, but keep in mind that the working orientation of LoRa monopole antennas is vertical.
<img width="975" height="459" alt="Screenshot 2026-08-14 at 16 28 20" src="https://github.com/user-attachments/assets/f294ca16-9855-479e-a185-3856b470e28f" />

