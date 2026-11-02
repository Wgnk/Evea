# Evea – Arduino-Based Human/Object Following Robot.

Evea is an Arduino-based smart robotic car designed to detect and follow a nearby person or object autonomously. Developed as part of our diploma engineering journey, the project combines embedded systems, sensor integration, wireless communication, and interactive robotics.
Equipped with ultrasonic and infrared sensors, a servo motor, Bluetooth connectivity, and an OLED display, Evea supports autonomous following as well as multiple modes of manual control through a smartphone.
The project demonstrates how different hardware components can work together to create an interactive and responsive robotic system.

# Project Overview:-

Evea is designed to operate in two primary modes:
1. Autonomous Mode: Scans its surroundings and follows a detected person or object using ultrasonic and IR sensor feedback.
2. Manual Control Mode: Allows users to control the robot through a Bluetooth-connected smartphone application using voice commands, gestures, or on-screen controls.
3. In addition, Evea monitors environmental temperature and humidity using a DHT11 sensor and transmits the readings wirelessly to a mobile application.
4. An OLED display adds an interactive element by displaying animated robotic eyes and facial expressions.

# Key Features :-

1. Autonomous Following ->
Detects and follows nearby objects or people using ultrasonic and IR sensors.

2. 180° Environment Scanning ->
Uses a servo-mounted sensor assembly to scan the surrounding area.

4. Voice Control ->
Supports voice-based commands through a Bluetooth-connected mobile application.

5. Gesture Control->
Allows movement control through supported smartphone gesture inputs.

6. Bluetooth Remote Control ->
Provides manual control through an Android application.

7. Temperature Monitoring ->
Measures ambient temperature using the DHT11 sensor.

8. Humidity Monitoring ->
Measures environmental humidity using the DHT11 sensor.

9. Wireless Data Transmission ->
Sends temperature and humidity readings through the HC-05 Bluetooth module.
10. Interactive OLED Display ->
Displays robotic eyes and facial expressions to make Evea more engaging.

# Hardware Components :- 

1. Arduino Uno ->
Main microcontroller responsible for processing sensor inputs and controlling the robot.

2. Motor Driver Shield ->
Controls the robot's motors and movement.

3. Ultrasonic Sensor ->
Measures the distance between the robot and nearby objects.

4. IR Sensors (2) ->
Assist with object detection and tracking.

5. Servo Motor ->
Rotates the sensor assembly to scan the surrounding area.

6. HC-05 Bluetooth Module ->
Enables wireless communication between the robot and smartphone.

7. DHT11 Sensor ->
Measures temperature and humidity.

8. OLED Display ->
Displays animated robotic eyes and expressions.

9. DC Motors and Robot Chassis ->
Provide the mechanical structure and movement.

10. Battery Supply ->
Provides power to the robotic system.

# Software and Technologies :-

-> Arduino IDE – Development and uploading of the firmware.
-> Embedded C/C++ – Programming the robot's control logic.
-> Arduino Libraries – Used for interfacing with sensors, the servo motor, Bluetooth communication, and OLED display.
-> Bluetooth Serial Communication – Enables wireless data exchange and remote control.
-> Arduino BlueControl – Used for Bluetooth-based control and displaying sensor readings.
-> Sensor Integration – Combines readings from ultrasonic and IR sensors for object detection and following.

# How Evea Works :-

1. Environment Scanning
When powered on, Evea uses a servo motor to rotate its sensor assembly across an approximately 180-degree field of view.
The ultrasonic and IR sensors collect information about nearby objects during this scanning process.
2. Object Detection and Following
Once a suitable target is detected, the Arduino processes the sensor readings and controls the motors through the motor driver shield.
Based on the detected position and distance, Evea adjusts its movement to follow the target.
3. Bluetooth-Based Control
Evea also supports manual operation through an HC-05 Bluetooth module.
A smartphone application can be used to control the robot through:
Voice commands
Gesture-based inputs
On-screen movement controls
This provides an alternative to autonomous operation.
4. Temperature and Humidity Monitoring
The DHT11 sensor continuously measures the surrounding temperature and humidity.
The readings are processed by the Arduino and transmitted through the HC-05 Bluetooth module to the connected smartphone application. We used Arduino BlueControl to display the received data in its application terminal.
5. Interactive OLED Display
The OLED display shows robotic eyes and facial expressions, giving Evea a more interactive appearance.
This feature adds a human-friendly interface and improves the overall user experience.
System Architecture

The overall system follows this structure:
                  SMARTPHONE
                      |
                      |
                 HC-05 Bluetooth
                      |
                      |
                 ARDUINO UNO
                      |
        +-------------+-------------+
        |             |             |
        |             |             |
   Motor Driver   Servo Motor   OLED Display
        |             |
        |        +----+----+
        |        |         |
     DC Motors  Ultrasonic  IR Sensors
                  Sensor   (2 Sensors)

                 DHT11 Sensor
                      |
                      |
                 ARDUINO UNO
                      |
                      |
               Bluetooth Data
                      |
                      |
              Smartphone App
# Working Modes :-

->> Autonomous Mode
Evea scans its surroundings, detects a nearby target, and adjusts its movement based on sensor feedback.

->> Voice Control Mode
The user can issue supported voice commands through a Bluetooth-connected smartphone application.

->>Gesture Control Mode
The robot responds to supported gesture inputs from the mobile application.

->>Manual Remote Control Mode
The user can directly control the robot's movement using on-screen buttons.

# Challenges Faced During Development :-

Building Evea involved several hardware and software integration challenges.
1. Sensor Synchronization
Integrating the ultrasonic sensor, IR sensors, and servo motor required coordinating multiple sensor readings to improve object detection and tracking.
2. Motor Control and Movement Stability
Achieving smooth movement while responding to changing sensor readings required adjustments to the motor control logic.
3. Multiple Control Modes
Integrating autonomous movement with voice, gesture, and manual Bluetooth control required managing different input sources within a single system.
4. Wireless Communication
Establishing reliable communication between the HC-05 module and the mobile application was important for receiving commands and transmitting environmental data.
5. Interactive Display
Integrating animated robotic expressions on the OLED display added another layer of functionality while coordinating the display with the robot's other operations.

# Future Improvements :-

-> Although Evea currently uses ultrasonic and IR sensors for object detection and following, several improvements could extend its capabilities.
-> Camera Integration: Add a camera module to capture visual information about the surroundings.
-> AI-Based Person Detection: Explore machine learning and computer vision for more reliable human detection.
-> Improved Target Tracking: Implement more advanced tracking algorithms to maintain a target even when it changes direction.
-> Obstacle Avoidance: Improve navigation by detecting and avoiding obstacles in the robot's path.
-> IoT Connectivity: Add Wi-Fi connectivity for remote monitoring and control.
-> Voice Interaction: Explore more advanced voice recognition and response capabilities.
-> Battery Monitoring: Integrate a battery-level monitoring system to indicate remaining power.
-> These enhancements could help transform Evea into a more capable autonomous robotic platform.

# Potential Applications :-

The concepts demonstrated in Evea could be extended to several real-world applications:
->> Healthcare Assistance: Experimental platforms for carrying lightweight items in controlled indoor environments.
->>Elderly Assistance: Exploring person-following technology for indoor assistance.

 ->>Educational Robotics:
Demonstrating Arduino programming, sensor integration, and embedded-system design.
Interactive Robotics: Creating robots capable of responding to human commands.
Indoor Automation: Exploring autonomous movement and object-following concepts.

## Note: Evea is an educational prototype. It is not intended to replace certified medical, security, or assistive devices.
