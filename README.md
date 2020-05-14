⚠️ **Not actively maintained** ⚠️

SD Card Library Photon Compat
===

An Implementation of the Arduino/Sparkfun SD Card Library for the Particle Photon.

This library is a fork of the [Spark Core SD library](https://github.com/mumblepins/sd-card-library). The code has been modified so that it will compile for the Particle Photon by following these instructions in [this forum post solution](https://community.particle.io/t/photon-and-sd-card-library-error/14707).

## Pin Diagram

In my circuits I use Adafruit's microSD card breakout board so I've included both sets of pin configurations.

### SD Card Pin Diagram

![](http://i.imgur.com/G78juSt.png)

### Adafruit MicroSD Breakout

![](http://i.imgur.com/No8R6UP.jpg)

### Pin Connection Table

Blank cells indicate that you ought to configure you hardware and softwae to use the functionality they match to (card detect and 5V). Card detect is not supported by 'naked' SD cards, but is supported on the breakout board.

| SD Card | Breakout  | Photon  |
|---      |---        |---      |
| n/a     | CD        |         |
| SS      | CS        | A2      |
| MOSI    | DI        | A5      |
| MISO    | DO        | A4      |
| SCK     | CLK       | A3      |
| GND     | GND       | GND     |
| VCC     | 3V        | 3V      |
| n/a     | 5V        |         |

### My own circuit

I've got a potentiometer wired in A0 in this circuit. Not this has no impact on the SD card and is specific to my project.

![](http://i.imgur.com/eJ8RQj7.jpg)
