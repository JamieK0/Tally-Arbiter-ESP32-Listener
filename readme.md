# ESP32 Listener
An ESP32 listener for Tally Arbiter.

## Features
- Neopixel indicator lights for program and preview
- OLED screen for displaying messages
- Messages are sent to the OLED screen on the tally light unit by including "@" at the start of the message
- 3D printed case. CAD files are included
- Side and bottom attachment points for accessories. Coldshoe mount is included in the CAD files.

## Tally Arbiter

> A camera tally lights project capable of listening/fetching tally data from multiple sources or video switchers and arbitrating whether an end device is considered to be in Preview or Program. Supports many different switcher types and protocols as well as many types of tally output.

Learn more [here](https://github.com/josephdadams/TallyArbiter).

## Installation

### 3D Printing
Use the stl or 3mf files in the CAD folder for printing.
The stl files seperate the top and bottom peices. 
I printed my case in PLA and it has been working fine.
The top peice is to be printed in white to act as diffusion for the LEDs.
#### Recommended print settings
- 3 permiters
- 15% infill for the bottom peice
- No infill or solid infill for the top peice. This is to ensure the LED diffusion is smooth.
- The coldshoe mount should be printed with the tally connector face facing the built plate. Supports may be needed.

## License
Distributed under the MIT License.