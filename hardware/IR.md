# IR receiver/transmitter module for Lilka

Inspired by DIY module recommended by Bruce firmware developers https://tasmota.github.io/docs/IR-Remote/#related-projects

## Parts
Most common 38kHz IR receivers are TSOPxxx38. Typical pinout: OUT, GND, Vcc (protruding side up, left to right)
You could use nearly any 36-38kHz 3-pin IC, but check the Datasheet for pinout.
IR emitting LED could be scraped from any old TV or AC remote

## Compatibility
Bruce and other IR apps. App settings: IR RX pin 14, IR TX pin 21

## Inventory <pin name>
- IR Emitter - 940nm LED1<+,->
- IR Receiver TSOP4838 - IRR<OUT,GND,VCC>
- 2N222 transistor Q1<c,b,e>
- 22 Ω resistor R1<1,2>
- 1 kΩ resistor R2<1,2> 
- 20x80 prototype PCB (cut a half)
- female 12-pin header J1<1-12>
- thin copper wires

## Wiring
| Lilka J2 # | Lilka pin | Destination |
|------------|-----------|-------------|
| 1          | GND       |   Q1<e>     |
| 2          | 3V3       |   R1<1>     |
| ..         |           |             |
| 7          | 21        |   R2<1>     |
| 8          | 14        |   IRR<OUT>  |
| 9          | 13        |             |
| 10         | 12        |             |
| 11         | 3V3       |   IRR<VCC>  |
| 12         | GND       |   IRR<GND>  |

Interconnections:
Q1<b>   to R2<2>
Q1<c>   to LED1<->
LED1<+> to R1<2>

It's recommended to test your circuit on a breadboard first before soldering. Use phone camera to verify that IR emitter works.
Depending on IR LED used the R1 value might need to be reduced to 10 or 15 Ω for improved IR range.
