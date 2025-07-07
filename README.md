🚗🤖 Evea: The Human-Following Robot 🔥

Thrilled to share our recent Arduino-based robot project – Evea, developed as part of our diploma journey with a passionate and innovative team! This smart robotic car is designed to follow a human, and it's loaded with interactive and intelligent features! 🚶‍♂️➡️🤖

🔧 Project Highlights:

🔹 Hardware:
(a) Arduino Uno as the central controller
(b) Motor shield for controlling movement of robot
(c) Ultrasonic Sensor + Two IR Sensors mounted on a Servo Motor for scanning and object/person detection
(d) Bluetooth Module HC-05 for:
(i) Voice Control 🎤
(ii) Gesture Control ✋
(iii) App-Based Remote Control 📱
(iv) DHT11 Sensor to measure and send temperature & humidity data via Bluetooth to application terminal connected with arduino. (we have used Arduino BlueControl for printing data) 🌡️💧
(e) OLED Display showing robotic eyes with facial expressions, giving Evea a personality! 👀😊

🧠 Functionality:

Evea starts by scanning a 180° area using the servo-mounted sensors to detect a human/object. Once detected, it follows the target using real-time input from the ultrasonic and IR sensors. You can also take control manually via a mobile app using Bluetooth voice, gesture, or button controls.
Meanwhile, it constantly monitors temperature and humidity, showcasing how embedded systems can multitask efficiently in real-time environments. The OLED display enhances the visual appeal by mimicking robotic expressions!

📈 Tech Stack:

>Arduino IDE for embedded programming
>C/C++ (Arduino) for sensor integration and control logic
>Bluetooth communication protocols for app control
>Sensor fusion logic for accurate tracking and control

🚀 Challenges & Takeaways:

💡 Synchronizing sensor feedback with motion control
 💡 Handling multiple input modes (voice, gesture, remote)
 💡 Achieving a balance between responsiveness and stability
This project taught us the value of hardware-software integration, sensor fusion, wireless control systems, and the power of collaborative development. 💪

🧠 Any further modification:
We can add camera module and load AI,ML feature to it for better functionality.

🌟 Use Case:
 Such robots have potential in healthcare, elderly assistance, surveillance, and interactive robotics for indoor use.
