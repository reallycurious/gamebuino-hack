# gamebuino-hack (eagle cad files)
A diy clone of open source [gamebuino classic](http://legacy.gamebuino.com/wiki)

**Differences in hardware**
  - Hack is based on Atmega328 PDIP so it does not have A6 and A7 (PC6 and PC7) pins
  - Button C is moved to D5 (PD5) -> rebuilding all games and bootloader needed for this change to work
  - Battery sensor is moved to ADC3 (PC3) -> rebuilding all games are needed for this change to work
  - No ambient light sensor
  - No pwm control for background led


**Bootloader**
  - gamebuino requires a [custom bootloader](https://github.com/ghalfacree/Arduino-Sketches/tree/master/hardware/arduino/bootloaders/gamebuino_boot) for loading games from sd-card to work
  - gamebuino bootloader only supports fat16 formatted sd cards

**Schematic**
![Shematic](schematic.png)


**PCB**
![PCB](board.png)
