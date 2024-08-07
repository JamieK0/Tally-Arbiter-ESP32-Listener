# ESP32 Listener/Tally Light with OLED and Neopixels
An ESP32 listener for Tally Arbiter.
![Alt text](Images/IMG_9926.png)
![Alt text](Images/IMG_2181.jpg)
![Alt text](Images/IMG_9970.JPG)
![Alt text](Images/IMG_9930.jpeg)

## Features
- Neopixel indicator lights for program and preview
- OLED screen for displaying messages
- Messages are sent to the OLED screen on the tally light unit by including "@" at the start of the message
- 3D printed case. CAD files are included
- Side and bottom attachment points for accessories. Coldshoe mount is included in the CAD files.

## Tally Arbiter

> A camera tally lights project capable of listening/fetching tally data from multiple sources or video switchers and arbitrating whether an end device is considered to be in Preview or Program. Supports many different switcher types and protocols as well as many types of tally output.

Learn more [here](https://github.com/josephdadams/TallyArbiter).

## Bill of materials
- ESP32 development board
- 1.3 inch i2c OLED screen
- 6x neopixel LEDs
- 14x M3 4mm length (OD 4.5mm) heated inserts
- 6x M3 16mm hex socket grubscrews
- Black PLA filament
- White PLA filament
- Insulated copper wires

## Tools
- 3D printer
- Soldering iron
- Hot glue gun
- Hex key set

## Installation

### 3D Printing
Use the seperate 3mf files in the CAD folder for printing.
I printed my case in PLA and it has been working fine.
The top piece is to be printed in white to act as diffusion for the LEDs.
#### Recommended print settings
- 3 permiters
- 15% infill for the bottom piece
- No infill or solid infill for the top piece. This is to ensure the LED diffusion is smooth.
- The coldshoe mount should be printed with the tally connector face facing the built plate. Supports may be needed.

### Wiring
| ESP32 | OLED | Neopixels |
|-------|------|-----------|
| 3V    | VCC  | 5V        |
| GND   | GND  | GND       |
| D18   |      | DIN       |
| D21   | SCA  |           |
| D22   | SCK  |           |

### Programing the ESP32
Use the Ardunio IDE to program the ESP32. This [tutorial](https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/) is helpful for installing ESP32 boards in the IDE.
The Arduino IDE sketch file is in the esp32-neopixel-listener folder.

### Building the case
Use a soldering iron to melt the heated inserts into the holes in between the two parts of the case. Add heated inserts to the accessory attachment points as well.
The screen can be placed into its compartment. Use some hot glue to secure it in place if necessary.
The ESP32 can slide in on an angle before being pushed against the back of the case to hold it in place.
The neopixels sit above the ESP32.
Use the appropriately sized hex key to screw the grub screws into the heated inserts, attaching the two pieces of the case.

## Making your own accessories
Accessories can be connected using this template for the heated inserts alignment:
![Alt text](<Images/Accessory Template.png>)

## License
Distributed under the MIT License.
