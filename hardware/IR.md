# IR receiver/transmitter module for Lilka

Inspired by DIY module recommended by Bruce firmware developers https://tasmota.github.io/docs/IR-Remote/#related-projects

## Compatibility
Bruce and other IR apps

## Inventory <with pins>
- IR LED (scraped from any IR remote) - LED1<+,->
- IR Receiver 36-38 kHz - IRR<1,2,3>
- 2N222 transistor Q1<b,c,e>
- 100 Ohm resistor R1<1,2>
- 20x80 prototype PCB (cut a half)
- female 12-pin header J1<1-12>
- thin copper wires

## Wiring (TODO)
| Lilka J2 # | Lilka pin | Destination |
|------------|-----------|-------------|
| 1          | GND       | Q1<e>,IRR<3>|
| 2          | 3V3       | IRR<1>,R1<1>|
| 3          | RX (44)   |             |
| 4          | TX (43)   |             |
| 5          | 48        |             |
| 6          | 47        |             |
| 7          | 21        |             |
| 8          | 14        |             |
| 9          | 13        |             |
| 10         | 12        |             |
| 11         | 3V3       |             |
| 12         | GND       |             |

