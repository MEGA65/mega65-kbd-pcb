# MEGA65 MK-II Keyboard PCB Design

## Why a MK-II Keyboard?

The short answer is "Chipaggedon", the chip shortage caused by COVID-19 etc.  This means that we can't get the Lattice FPGA
part that was used on the original MEGA65 keyboards.

Also, we would like a keyboard PCB design that is easier for people to build themselves, if they want to.

## So how does it work?

The MEGA65 keyboard interface has 3 IO lines available. On the MK-I keyboard design, they are CLK/SYNC, OUT and IN.
We would like for the MEGA65 core to be able to auto-detect both models of keyboard. Based on parts that are easily
available at the moment, I have opted for using several I2C IO expanders, which means that we only need 2 lines.
The third line is tied low on the MK-II keyboard, which the MK-I keyboard will not do. This makes auto-detection possible.

## What about NKRO?

I opted to connect each key to a GPIO on an I2C IO expander, because this allows full NKRO, without requiring any
diodes on the board or in the keyswitches. This makes assembly easier, and probably cheaper.

## What do I need to build one?

You need to produce the gerber and drill files from the Kicad project in this repository if you want to get the PCB made
yourself.

After that, you will need:

2x 330 Ohm mini sized hole-through resistors for the CAPSLOCK and SHIFT LOCK keys.
12x 130 Ohm mini sized hole-through resistors for the RGB LEDs.
4x Wuerth RGB LEDs, two for each side. Part number is 156120M173000.
2x clicky Cherry MX(tm) or compatible key switches with LEDs.
76x Cherry MX(tm) or compatible key switches of the flavour of your choice. They don't need internal diodes.
1x 10-pin 2x5 2.54mm male pin header.
1x 4-pin 1x4 2.54mm male pin header, if you want to attach the optional GPIO header (it isn't used for anything right now).

... and a set of MEGA65 keycaps, or some other key caps to make do until we find a way to make the proper caps available.

## Any tips for assembly?

This is a new design, and we will update the instructions once we have built one.  
But the general tips apply:
1. Everything except for the key switches are attached to the "front" of the PCB, that has the MEGA65 logo on it.
2. The key switches are inserted on the "back". Each spot is marked, and the two that should have LED-fitted keys are marked for your convenience.
3. The surface-mount chips are not so small, so you should be able to hand solder them using tricks like bridge soldering, and then sucking the bridges away using a roll of solder wick.

## License

This PCB design is (C) Copyright Paul Gardner-Stephen, 2022, and is offered to you under the CC-BY-SA 4.0 license.

Open Hardware Certification has been applied for.

## Need help?

Go to https://mega65.org, and find the link to our Discord server, and ask the friendly community there for any help you might need.
