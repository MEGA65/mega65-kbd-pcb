
# How to assemble the DIY MEGA65 keyboard

## 1. Get the parts

Get the board from a reliable source or order some to your preferred manufacturer from this KiCad project.

* Inspect the board for any defect
![Component side of the board](images/mega65-kbd-pcb-back.png)
![Key switchs side of the board](images/mega65-kbd-pcb-front.png)

* Get the components from your preferred supplier
![Check components](images/mega65-kbd-components.png)
![Have your key switchs](images/mega65-kbd-components-keyswitches.png)

## 2. Assembly ( Get you soldering iron ready ! )

### 2.1 The RGB LEDs

### 2.2 The TCA/PCA9555s

### 2.3 The resistors

### 2.4 The connectors

### 2.5 The key switches

Place the standard key switches of your choice on the front side of the board, leaving out the Caps Lock and Shift Lock free.
Place the two "clicky" key switches at the Caps Lock and Shift Lock positions.
![Board with key switches](images/mega65-kbd-pcb-with-switches.png)

Return the board by placing a large cardboard on the switches, to prevent them from falling off if they don't have retaining studs.

Solder all the contacts.

### 2.6 Now is a good time to test the keyboard

Now that all major components are in place, you can hook up the keyboard with a 10 conductors flat cable to your MEGA65 board or your DIY FPGA board.

Start your MEGA65 and check that the new keyboard has been detected.
Go to the keyboard test utility, and try every key.

### 2.7 The "lock" switches LEDs

Insert the two 3mm LEDs in the dedicated holes of the clicky keys.
With the MEGA65 turned on, test the Caps Lock and Shift Lock keys to check that the LEDs toggle correctly.
If any LED doesn't illuminate, try reversing it in its slot. Polarity may have been wrong.

Once you're confident the lock LEDs work correctly, turn off the MEGA65, unplug the keyboard before soldering them.

### 2.8 The stabilizer bars

Place the Return and Space Bar stabilizer bars on the board, securing them gently with 2 screws on the back.

### 2.9 And finally, fit the keycaps

Now, I guess you didn't wait for this last step.
But if you did, it's now time to place all the keycaps on the board, and start enjoying your new keyboard !!!

## 3. Have fun !