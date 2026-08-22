# IR receiver/transmitter module for Lilka

Inspired by DIY module recommended by Bruce firmware developers https://tasmota.github.io/docs/IR-Remote/#related-projects

## Parts
Most common 38kHz IR receivers are TSOPxxx38. Typical pinout: OUT, GND, Vcc (protruding side up, left to right)
You could use nearly any 36-38kHz 3-pin IC, but check the Datasheet for pinout.
IR emitting LED could be scraped from any old TV or AC remote

## Compatibility
Bruce and other IR apps. App settings: IR RX pin 21, IR TX pin 14 

## Inventory <with pins>
- IR Emitter - LED1<+,->
- IR Receiver TSOP4838 - IRR<1,2,3>
- 2N222 transistor Q1<b,c,e>
- 100 Ω resistor R1<1,2>
- 1 kΩ resistor R2<1,2> 
- 20x80 prototype PCB (cut a half)
- female 12-pin header J1<1-12>
- thin copper wires

## Wiring
| Lilka J2 # | Lilka pin | Destination |
|------------|-----------|-------------|
| 7          | 21        | IRR<1>      |
| 8          | 14        | R2<1>       |
| 9          | 13        |             |
| 10         | 12        |             |
| 11         | 3V3       | IRR<3>,R1<1>|
| 12         | GND       | Q1<e>,IRR<2>|
|            |           | Q1<b>,R2<2> |
|            |           |Q1<c>,LED1<->|
|            |           |LED1<+>,R1<2>|

It's recommended to test your circuit on a breadboard first before soldering. Use phone camera to verify that IR emitter works.