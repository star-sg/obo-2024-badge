# Off-By-One Conference 2024

## Hardware Badge

These are the instructions on how to get started and hack your badge. The hardware badge consists of multiple microcontrollers with capture-the-flag challenges.

***[Conference Badge.pdf](<Conference Badge.pdf>)***

These are the solutions to the challenges on the badge.

***[Solution](./Solution)***

This is the firmware for the glitch target. Take note that the target is running on a 3V3 logic level, and you may reflash using the following commands.

```
# Fuses
avrdude -c avrisp -patmega328p -e -Ulock:w:0xff:m -Uefuse:w:0b11111111:m -Uhfuse:w:0xd7:m -Ulfuse:w:0xe2:m
# Sketch
avrdude -c avrisp -patmega328p -Uflash:w:target_arduino.ino.hex:i
```

## Soldering Workshop

This guide will tell you how to assemble your LED Name Tag Kit at the Off-By-One conference. This project is suitable for beginners to learn about soldering techniques 

***[Soldering Workshop Guide.pdf](<Soldering Workshop Guide.pdf>)***

