# smart-dustbin
This project demonstrates how to create a smart dustbin using an Arduino Uno microcontroller, an IR (Infrared) sensor, and a motor. 
The IR sensor detects the presence of an object near the dustbin, and the motor is used to open and close the dustbin lid automatically.

Components Required:
Arduino Uno
IR sensor
servo Motor
Jumper wires(for connection )
Breadboard

Code Explanation:
Dustbin or enclosure
Define the pin numbers for the IR sensor and the motor.
Initialize the serial communication for debugging purposes.
Set the pin modes for the IR sensor as input and the motor as output.
In the loop() function, read the state of the IR sensor using the digitalRead() function.
If an object is detected (IR sensor reads HIGH), call the openDustbinLid() function to open the dustbin lid.
If no object is detected (IR sensor reads LOW), call the closeDustbinLid() function to close the dustbin lid.
The openDustbinLid() function sets the motor pin to HIGH, which rotates the motor to open the lid.
The closeDustbinLid() function sets the motor pin to LOW, which stops the motor and closes the lid.

Usage:

Connect the IR sensor and motor to the Arduino Uno following the circuit diagram.
Upload the code to the Arduino Uno using the Arduino IDE.
Open the Serial Monitor to observe the status of the dustbin lid (open or closed) when an object is detected.
Test the project by placing an object in front of the IR sensor. The dustbin lid should open automatically.
