# H-bridge-and-DC-Motor-

Project Introduction:
This project involves controlling a DC motor using an Arduino. The goal is to demonstrate basic motor control techniques, including starting, stopping, and reversing the direction of the motor. This is achieved through the use of a motor driver circuit which allows the Arduino to manage the motor's operation via digital output pins.

Connections:
Enable Pin (Pin 10): This pin is used to enable or disable the motor driver. Connecting it to a high value (255 in this case) ensures the motor driver is active.
Motor Pins (Pin 7 and Pin 8): These pins control the direction of the motor. MotorPin1 (Pin 7) and MotorPin2 (Pin 8) are connected to the inputs of the motor driver. Depending on which pin is HIGH, the motor will rotate in a specific direction or stop.
How It Works:
In the setup() function, the pins are initialized as outputs, and the motor is initially stopped by setting both motor control pins to LOW. The analogWrite function is used to set the enable pin to a high value, allowing the motor driver to be active.
In the loop() function, the motor is controlled by setting the pins to HIGH or LOW in a sequence that alternates the motor's direction every 5 seconds. This creates a pattern where the motor rotates in one direction, stops, then rotates in the opposite direction, and stops again.
Overall, this project demonstrates basic motor control using an Arduino and a motor driver, suitable for various applications requiring simple motor actuation.
