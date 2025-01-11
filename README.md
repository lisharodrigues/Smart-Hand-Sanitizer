# Automatic Hand Sanitizer

This project demonstrates an automatic hand sanitizer dispenser using an ultrasonic sensor and a servo motor. 

**How it works:**

1. **Sensor Detection:**
   - An ultrasonic sensor (HC-SR04) is used to detect the presence of a hand. 
   - The sensor emits a sound wave and measures the time taken for the echo to return.
   - If the distance between the sensor and the hand is less than a predefined threshold (e.g., 5 cm), it indicates that a hand is present.

2. **Sanitizer Dispense:**
   - A servo motor is attached to the sanitizer bottle.
   - When the sensor detects a hand, the servo motor rotates 180 degrees.
   - This rotation triggers the release of a small amount of sanitizer.

3. **Reset:**
   - After a short delay, the servo motor returns to its original position, preparing for the next use.

**Hardware Components:**

* Arduino board (or compatible microcontroller)
* Ultrasonic sensor (HC-SR04)
* Servo motor
* Jumper wires
* Breadboard (optional)
* Sanitizer bottle with a suitable dispenser mechanism

**Software:**

* Arduino IDE

**Connections:**

* **Ultrasonic Sensor:**
    - VCC to 5V
    - TRIG to digital pin 5
    - ECHO to digital pin 4
    - GND to GND
* **Servo Motor:**
    - Signal to digital pin 3
    - VCC to 5V
    - GND to GND
