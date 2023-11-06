# ArduinoSumoRobot

1. Theme syncretic project
A microcontroller-based minisumo robot type system will be created using:
● A driver for controlling DC motors via PWM.
● Two DC motors with wheels.
● A distance sensor to detect the opponent or obstacles.
● A line sensor to detect the edge of the arena.
● An LED to display the operating status.
● A battery for power supply.
● Max robot dimensions: L=10cm xh=10cm xl=10cm, and weight < 0.5Kg.
2. Development stages
● Presentation 1-PWM (presents in week 5):
Using a microcontroller timer, generate a PWM signal on both channels of the 
selected timer. The filling factor will be given through the serial interface in the 
format: "<filling factor channel A>A <filling factor channel B>B".
(Ex.. on receiving "90A 45B" from the PC will generate a PWM with 90% duty factor 
on channel A and a signal with 45% duty factor on channel B).

Obs. Engines are not required for this theme. Checking the PWM signal will be done 
with an LED connected to channels A and B of the chosen timer.
● Presentation 2-Distance sensor (presents in week 7):
Using timers calculate and display on the serial interface the distance obtained from the 
ultrasonic sensor. (see examples). Theme 2 is implemented as a continuation of the project 
started for the first theme (ie. the PWM signal is functional and can be modified via the 
serial interface).
● Presentation 3-Line sensor (presents in week 8):
Implement a function to read the line sensor and control an LED so that it is lit 
when the line sensor detects exiting the arena (ie detects a white surface).
●
along with theme 5)
Presentation 4-Engines + chassis construction (shown in week 11
Presentation of the final construction that falls within the constraints defined in the first 
week (max. dimensions: 10cm x 10cm x 10cm, weight < 500g).
● Presentation 5-Internal Logic (presents in week 11)
a. The robot will start from the center of the arena (matte black type surface).
b. It will wait 3 seconds in idle position.
c. It will rotate in place (equal speeds in the opposite direction on the two motors) 
until the distance sensor detects an obstacle (a 5x5x5cm polystyrene cube).
d. After detecting the obstacle the robot will move towards it and push it until the 
line sensor detects leaving the arena (white striped border).
e. Step c is resumed.
Presentation of themes 5 and 6 is done according to the entries in the document below:
● Presentation 6-Final presentation (due in week 13)
3. FAQ
Example components:
● 1 x Arduino Nano
● 2 x DC motor
● 2 x Plastic Wheel with Rubber with a diameter of 27 mm
● 1 x Prototyping board Test harness 70 x 90 mm (for connections and chassis)
● 2 x TIP31C or Dual Motor Driver Module (10 V, 1.5 A)
● 1 x Infrared Line Sensor
● 1 x HC-SR04 ultrasonic sensor
● 1 x 9V Battery Holder
● 1 x 9V battery