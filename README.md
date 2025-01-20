# Line_Follower_Robot_project(5 IR Sensors)
This project demonstrates a line follower robot equipped with five IR sensors for precise line tracking. The repository includes:

   The track layout used for testing (uploaded by the user),
   Details of the IR sensor placement and configuration,
   A custom algorithm implementing feedback control for accurate line following, ensuring stability and smooth navigation,
   Comprehensive documentation on hardware setup, software implementation in Arduino IDE.

This project serves as an excellent reference for robotics enthusiasts and beginners exploring sensor-based feedback control systems.
The numbers in the track are for evaluation purposes, so just ignore them...

<u>Here is the connection details</u><br>
IR Sensors Connections,<br>
The code defines the following pins for IR sensors:<br>
IR_SENSOR_RIGHTMOST: Pin 12<br>
IR_SENSOR_RIGHT: Pin 11<br>
IR_SENSOR_MID: Pin 4<br>
IR_SENSOR_LEFT: Pin 3<br>
IR_SENSOR_LEFTMOST: Pin 2

Wiring:<br>
Connect the OUT pin of each IR sensor to the respective Arduino pin as defined above.<br>
Connect the VCC pin of the IR sensors to 5V on the Arduino Nano.<br>
Connect the GND pin of the IR sensors to the GND on the Arduino Nano.

Right Motor Pins:<br>
Enable Pin: Pin 6 (PWM)<br>
Input Pins:<br>
Pin 10 → IN1 (Right motor forward)<br>
Pin 8 → IN2 (Right motor backward)<br>
Left Motor Pins:<br>
Enable Pin: Pin 5 (PWM)<br>
Input Pins:<br>
Pin 9 → IN3 (Left motor forward)<br>
Pin 7 → IN4 (Left motor backward)<br>

Connect the Enable pins (ENA and ENB) of the L298 to pins 6 and 5 respectively on the Arduino.
Connect the IN1, IN2, IN3, and IN4 pins of the L298 to pins 10, 8, 9, and 7 respectively on the Arduino.
Connect the motor terminals to the motor output pins of the L298:<br>
Right Motor: OUT1 and OUT2<br>
Left Motor: OUT3 and OUT4<br>
Connect the VCC pin of the L298 to an external power source (typically 12V or according to your motor's requirement).
Connect the GND pin of the L298 to the common ground (shared with Arduino).
Connect the 5V output pin of the L298 to the 5V pin on the Arduino Nano.

A battery pack (e.g., 6V or 12V) is used to power the motors through the L298 motor driver's VCC pin.
Ensure the ground of the battery is connected to the common ground shared by the Arduino Nano and L298.

Connect the Arduino Nano USB port to your PC for programming.
Power the Arduino Nano either through the USB port or by connecting the VIN pin to the L298 motor driver's 5V output.

Ensure you have a common ground connection between all components (Arduino, L298, and sensors).
If motors consume high current, use a heat sink with the L298 motor driver.

The circuit must be like this,(it depends upon the user what pins he takes:),
![LFR using 5 ir sensor sketch](https://github.com/user-attachments/assets/16ffd835-c851-4a2b-9569-fbb1e422c64c)







   
