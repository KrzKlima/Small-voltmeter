# Small-voltmeter
The project and all files in this repository are provided under CC BY-NC-SA 4.0 license.

This voltmeter is small (I mean, small), cute, fits on a breadboard and is powered from a 3v3 voltage supply. It even includes a Zener voltage regulator, but for larger supply voltages a dropper resistor is required (0402 resistors have weak power capabilities). The use of bubble display makes reading the voltage easy, despite the minute size of the digits. It uses ATTiny44A and MCP3421 ADC. The board size is 20.5mm by 10.5mm.

The measurement ranges are the following:
1) -2V to 10V with the resolution of 1mV
2) outside the range 1), within -20 to 100V, with the resolution of 10mV
3) outside the ranges 1) and 2), within -200 to 200V, with the resolution of 100mV
(but you need to observe the safety issues with such high voltages)



Highlights:
- small form factor ~DIP16
- due to the low pin count of the MCU, I2C bus to the external ADC is multiplexed with display outputs - and it still works!
- differential input
- measures ground referenced voltages of both polarities

Two videos showing the operation of the multimeter are linked below.

[![SAMPLE VIDEO 1](http://img.youtube.com/vi/5PMVABGqFHo/0.jpg)](https://www.youtube.com/watch?v=5PMVABGqFHo "Small multimeter - video 1")
[![SAMPLE VIDEO 2](http://img.youtube.com/vi/kH4eJVx0Qz0/0.jpg)](https://www.youtube.com/watch?v=kH4eJVx0Qz0 "Small multimeter - video 2")
