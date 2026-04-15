Counter-Using-IR-Sensor
object counter which uses IR Sensor to count the number of passing objects and displays the count on an LCD Screen

This project uses an Arduino and an IR sensor to count objects and show the total on an LCD screen. 
Instead of checking the sensor over and over, the code uses a "hardware interrupt." This means the Arduino watches the sensor in the background. When an object passes by, the Arduino reacts instantly to count it, ensuring it never misses a fast-moving item. 
To keep the count accurate, the code includes a short timer to ignore any sensor glitches that might cause double-counting. Once the object is securely counted, the Arduino updates the screen.

What You Need
Arduino (Uno, Nano, or similar)
IR Obstacle Avoidance Sensor Module
16x2 LCD Display with an I2C backpack
Jumper wires
Breadboard

Wiring Guide

IR Sensor:
VCC - 5
GND - GND
OUT - Digital Pin 2

I2C LCD
VCC - 5V
GND - GND
SDA - A4
SCL - A5 
