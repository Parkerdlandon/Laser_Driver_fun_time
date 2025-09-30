# Reverse Engineering Calmar Laser Inc. PCB: 1003598 PCBA: 1003599
Attempting to reverse engineer a laser diode driver

# Notes about ICs on board

## Pump Diode
- [L4 915/940/975 nm Fiber-Coupled Laser](https://resource.lumentum.com/s3fs-public/technical-library-items/6398l4l4i-ds-cl-ae.pdf?VersionId=null)

## Relevant ICs
| On board label | Package | Name & Datasheet link|
| ---            | ---     | ---                  |
| **U1,U4** | SOIC8     | [LM393 - Dual Differential Comparator](https://www.ti.com/product/LM393#pps)|
| **U3,U5** | SOIC8     | [LMC648 - CMOS Rail-to-Rail opAmp](https://www.ti.com/lit/ds/symlink/lmc6484.pdf)|
| **U2**    | DIP 16    | [SNx4 HC04 - Hex Inverters](https://www.ti.com/lit/ds/symlink/sn74hc04.pdf)|
| U7        | DIP 16-Wide? | [TEC5V6A - High Efficiency TEC controller](https://www.analogtechnologies.com/document/TEC5V6A-D.pdf)|
| **U9**    | DIP 16    | [HC00 - Quad input Nand gate](https://www.ti.com/lit/ds/symlink/sn74hc00.pdf)|
| **U10**   | DIP 16    | [HC175 - Quad D-Flip-Flop](https://www.alldatasheet.com/datasheet-pdf/pdf/2081107/SS/54HC175.html)|
| **U11**   | SOT23-6   | possibly [SN74LVC1G332 - Single 3 input positive or gate](https://www.ti.com/lit/ds/symlink/sn74lvc1g332.pdf?ts=1759128521935&ref_url=https%253A%252F%252Fgoogle.com%252F)|
| U13   | ?         | [ECS-8FM-040 4.000MHz Oscillator\*](https://www.mouser.com/datasheet/3/294/1/ecs-8f.pdf)|

\**This has been updated to meet RoHS standards: [Product Change by ECS](https://ecsxtal.com/store/pdf/100920-ECS-8F-PCN.pdf)*

## Passive Components

- SOME LASER DIODE??? 0110E 6169 ???? maybe?

| On board label | Package | Name & Datasheet link|
| ---            | ---     | ---                  |
| **Q1**         | TO-220  | [IRL3302 - Power MOSFET](https://www.mouser.com/catalog/specsheets/irl3302.pdf)|
| **D4, D5, D6, D7** | TO-220 | [MBR60100CT - SCHOTTKY RECTIFIER](https://www.smc-diodes.com/propdf/MBR60100CT%20N0777%20REV.B.pdf)|



### Resistors
| On board label | Name & Datasheet link |
| ---            | ---                   |
| **R26, R27**   | [50 Ohm Power resistors](https://www.digikey.com/en/products/detail/ohmite/15FR050E/822916)|
