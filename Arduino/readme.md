==Arduino Mega interface to Replica 1+ keyboard socket==

Data Logger Shield connects on top of Mega and contains an SD card.
Place text files of code to be sent to Apple1 in /apple1/ directory.
LCD button shield connects on top of Data Logger Shield.

Pin wiring:
MEGA +5V is not used but may be wired to breadboard.

- MEGA --> REPLICA1
- 23 --> 2 (Strobe)
- 25 --> 5 (D5)
- 27 --> 6 (D4)
- 29 --> 7 (D6)
- 31 --> 19 (D2)
- 33 --> 11 (D3)
- 35 --> 12 (D0)
- 37 --> 13 (D1)
- GND --> 8 (GND)

Use a 16 pin ribbon cable to connect breadboard to Replica 1 socket.
I have found that I need to unplug the cable from the Replica 1 when powering it on.
First, prepare the Replica 1 to receive either a hex dump or basic program.
For a hex dump, press Reset and hit enter a few times.
For Basic, make sure the jumper is set correctly for Integer Basic or Applesoft.
Then type E0000R then hit enter a few times.
Then connect the cable to the Replica 1 socket and power on the Arduino via USB or the barrel jack.
Use the Up and Down buttons to scroll through the list of files in the /apple1/ directory.
Click the Select button to start sending the displayed text file to the Replica 1.
Have Fun!
