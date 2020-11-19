Saturn Switchless Mod (COMMON ANODE R-G LED)
=============================================

This is the PIC-code needed for the Switchless Mod as described at http://knzl.de/saturnmod/ .

BUT IN THIS CASE IS MADE FOR COMMON ANODE RED-GREEN LED USED TO SWITCH ORIGINAL CONSOLE POWER LED.
Instead of using original saturn LED gnd pad, you have to use its positive (+vcc) pad to solder common anode to it.
Then both cathodes to pins 5 (red led leg) and 6 (green led leg) of the PIC 16F630.
You can add a 220 Ohm resistor from pin 5 to red leg of the led in order to soften that color to get a more defined orange one when both parts of the led are lighted.
Don't use original led anode hole on the pcb for the R-G anode, search for a real 5v source.

For flashing a 16F630 (maybe 16F676 but untested), you will only need the .hex-file, the rest is
the source-code needed for building it yourself.
I've added both hex, original common cathode led and this modified for common anode leds.

COLORS: Red = JAP, Orange = USA, Green = PAL

BLINKING LED: Slow = 50hz, Fast = 60hz

Building
--------

For building it, you'll need:

 * Microchip MPLAB IDE (FREE) with included HI-TECH C Compiler (http://ww1.microchip.com/downloads/en/DeviceDoc/MPLAB_8.30.zip)
 
License
-------

    Saturn Switchless Mod
    Copyright (C) 2004 Sebastian Kienzl
    Modified by yavimaya 2020.
    
    This program is free software; you can redistribute it and/or
    modify it under the terms of the GNU General Public License
    as published by the Free Software Foundation; either version 2
    of the License, or (at your option) any later version.
    
    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

