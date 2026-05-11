# Vibrating Directional Gloves (VDG)

## Overview

The Vibrating Directional Gloves (VDG) project aims to enhance driving safety by providing tactile feedback for GPS directions. These gloves utilize haptic feedback to indicate 'turn left' and 'turn right' commands, making driving safer and more intuitive. The project integrates speech recognition and vibration motors controlled by an Arduino Nano 33 BLE Sense.

## Project Contributors

- Daivya Shah (dts7992@nyu.edu)
- Kaylee Weber (kew6119@nyu.edu)
- Jiangnan Wang (jw7572@nyu.edu)

## Project Advisors

- Professor Rui Li (rui.li@nyu.edu)

## Features

- **Tactile Feedback**: Provides vibrations on the left or right glove to indicate GPS directions.
- **Speech Recognition**: Utilizes Edge Impulse for training models to recognize 'turn left' and 'turn right' commands.
- **Arduino Integration**: Uses Arduino Nano 33 BLE Sense to process and execute commands.

## Components

### Hardware
- Arduino Nano 33 BLE Sense
- Vibration Motors
- Breadboard, wires, resistors, diode rectifier, NPN transistor, 3V power source
- 3D-printed frame for housing components
- Nike sock used to create a comfortable and low-cost glove

### Software
- **Edge Impulse**: For collecting and training speech samples.
- **Arduino IDE**: For programming the Arduino Nano 33 BLE Sense.

## Installation

### Hardware Setup
1. Assemble the circuit on the breadboard with Arduino Nano 33 BLE Sense, vibration motors, and other components.
2. Secure the Arduino and components in the 3D-printed frame.
3. Attach the frame to the glove made from a Nike sock using Velcro.

### Software Setup
1. Train the speech recognition model on Edge Impulse with samples of 'turn left', 'turn right', and 'noise'.
2. Download the trained model from Edge Impulse as an Arduino library.
3. Install necessary libraries in Arduino IDE:
   - `Adafruit_ZeroPDM-Master`
   - `Arduino BLE-1.3.2`
   - `Project2_inferencing` (downloaded from Edge Impulse)
4. Upload the code to Arduino Nano 33 BLE Sense.

## Usage
1. Wear the gloves and connect the Arduino to a power source.
2. The gloves will vibrate based on the GPS commands 'turn left' and 'turn right' recognized by the speech recognition model.

## Project Schedule and Costs

### Schedule
- **Start Date**: October 9
- **End Date**: November 10
- **Advanced Functions and Extra Credit**: Post-November 10

### Cost Breakdown
- **Initial Estimate**: $7,640
- **Final Cost**: $2,540.59

## Challenges and Solutions
- **Vibration Motor Circuit**: Issues with wiring diagrams were resolved through research and planned capacitor addition.
- **Speech Recognition**: Limited experience required extensive experimentation with Edge Impulse.

## Future Improvements
- Enhance the device to read numerical signals for more detailed feedback.
- Expand applications for visually or auditory-challenged individuals.

## References
- [How We Feel Touch](https://askabiologist.asu.edu/explore/how-do-we-feel-touch)
- [Response Time to Stimuli](https://www.iaeng.org/publication/IMECS2012/IMECS2012_pp1449-1454.pdf)
- [US Drivers Statistics](https://usafacts.org/data/topics/people-society/transportation/safety/licensed-drivers/)
- [GPS Dependency](https://www.carpro.com/blog/where-drivers-are-most-dependent-on-gps-systems)
- [Circuit Diagram](https://www.circuito.io/app?components=514,8449,11022)
- [Speech Recognition with Arduino](https://circuitdigest.com/comment/33907#comment-33907)
