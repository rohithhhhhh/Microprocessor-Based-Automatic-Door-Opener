# Microprocessor-Based Automatic Door Opener

This project is an implementation of an automatic door opener using an Arduino microcontroller, an IR sensor, and a servo motor. When an object is detected by the IR sensor, the door automatically opens by rotating the servo motor, and LEDs indicate the status (open/close).

## Features
- **Automatic Door Opening**: The door opens when an object is detected by the IR sensor.
- **Visual Indicators**: Green LED turns on when the door is open, and Red LED turns on when the door is closed.
- **Servo Motor Control**: Controls the door opening mechanism.

## Components Required
- Arduino (or compatible microcontroller)
- IR sensor
- Servo motor
- Green LED
- Red LED
- Resistors (220Ω for LEDs)
- Jumper wires
- Breadboard

## Circuit Diagram
1. **IR Sensor**: Output pin connected to Arduino pin 2.
2. **Green LED**: Connected to Arduino pin 5.
3. **Red LED**: Connected to Arduino pin 6.
4. **Servo Motor**: Signal pin connected to Arduino pin 3.

## How it Works
1. The IR sensor detects an object. When the object is detected, it sends a HIGH signal to pin 2 of the Arduino.
2. When the signal is HIGH:
   - The Green LED turns on.
   - The Red LED turns off.
   - The servo motor rotates 90° to open the door.
3. When no object is detected (signal is LOW):
   - The Green LED turns off.
   - The Red LED turns on.
   - The servo motor rotates back to 0° to close the door.

## Installation and Setup
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/rohithhhhhh/Microprocessor-Based-Automatic-Door-Opener.git
   ```
2. Open the Arduino IDE and load the `code.c` file.
3. Connect the circuit as per the diagram and upload the code to the Arduino.
4. Open the Serial Monitor in Arduino IDE to view sensor output.

## License
This project is open source and available under the MIT License.
