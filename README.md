"Hand Gesture Controlled Car (HGCC)," 
Project Title
Hand Gesture Controlled Car 

Objective
To design and implement a car that can interpret hand gestures to control its movements wirelessly using Arduino and an RF module.

Team and Guidance
Institute: Shri Ram Institute of Technology, Jabalpur (B.Tech AIML)
Project Incharge: Prof. Supriya Shrivastava
Project Guide: Prof. Rahul Chelani
Team Members:
Mehul Vishwakarma (Leader)
Ayush Jaiswal
Abhay Sahu
Kashish Patel​
Components Used
Arduino NANO
Arduino UNO
L298N Motor Driver
RF Module
Car Chassis
ROOFER INR 18650 25000 mAh Battery
Gear Motor
Wheels
Connectors
PCB
Adaptor
Soldering Wire
Glove
Velcro Tape​
​
Key Devices
Arduino Nano: Microcontroller board for gesture recognition.
Arduino Uno: Microcontroller board for processing and controlling the car's movements.
L298N Motor Driver: Controls speed and direction of the DC motors using PWM signals.
MPU-6050 Accelerometer: Detects hand gestures based on acceleration and motion data.
RF Module: Wireless communication between the transmitter (glove) and receiver (car).​
​
Working Mechanism
Gesture Detection:
The glove with an MPU-6050 accelerometer detects hand movements like tilts (forward, backward, left, right).
Signal Transmission:
The Arduino Nano processes gesture data and converts it into commands (e.g., "FORWARD").
Commands are sent wirelessly via the RF module.
Signal Reception:
The Arduino Uno in the car receives commands from the RF module.
The motor driver interprets the commands to control motor movements.
Car Movements:
Tilts in the glove result in respective car actions (move forward/backward, turn left/right, stop).​
​
Circuit Design
Transmitter: Glove-based system with MPU-6050, Arduino Nano, and RF module.
Receiver: Car-based system with Arduino Uno, L298N motor driver, and RF module.
Connections:
RF transmitter to Arduino Nano.
RF receiver and motor driver to Arduino Uno.
Motors to L298N motor driver.​
​
Programming Overview
Transmitter Code (Glove):

Reads acceleration data from the MPU-6050.
Converts gestures into commands like "FORWARD," "BACKWARD," etc.
Sends commands wirelessly via the RF module.
Receiver Code (Car):

Receives commands from the RF module.
Interprets commands to control motor actions using L298N motor driver.
Commands include forward, backward, left, right, and stop.
Example Functions:

moveForward(): Activates motors to move forward.
turnLeft(): Activates specific motors for left turn.​
​
Expected Output
Car moves as per the hand gestures:
Forward tilt: Car moves forward.
Backward tilt: Car reverses.
Left tilt: Car turns left.
Right tilt: Car turns right.
Neutral position: Car stops.​
​
Deliverables
Working prototype of the hand gesture-controlled car.
Demonstration of seamless communication between glove and car.
Functional responsiveness to all gestures.
