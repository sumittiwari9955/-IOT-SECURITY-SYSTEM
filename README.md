# COMPANY:- CODTECH IT SOLUTION
# NMAE:- SUMIT KUMAR
# INTERN ID:- CT04DF1595
# DOMAIN:- Internet Of Things
# DURATION:- 4 WEEKS
# MENTOR:- NEELA SANTOSH
# DESCRIPTION #
# OUTPUT:-
https://github.com/user-attachments/assets/df09549f-9520-40d6-b946-14d59b2654a6
https://github.com/user-attachments/assets/46163667-d7d0-4405-bf10-041050682369
IoT-Based Security System Using ESP32-CAM and PIR Motion Sensor

This project demonstrates an efficient and low-cost IoT-based security system using the ESP32-CAM module. The system is designed to detect motion using a PIR sensor, capture images with the ESP32-CAM, and send real-time alerts to a mobile application. This solution is ideal for home or small-office surveillance, providing enhanced security through automation and remote monitoring.

Hardware Components Used
ESP32-CAM Module
The ESP32-CAM is a low-cost development board that combines the ESP32-S microcontroller with a built-in OV2640 camera. It supports Wi-Fi and Bluetooth connectivity, making it suitable for IoT applications. The board includes a microSD card slot, multiple GPIOs, and a reset button. It is the core of the project, responsible for image capturing, motion detection control, and Wi-Fi communication.

ESP32-CAM Programmer (USB to TTL Adapter)
The ESP32-CAM lacks a built-in USB interface, so an external programmer is necessary. This is typically a USB to TTL serial adapter, such as the FTDI FT232RL USB to Serial Adapter or CP2102 USB to UART Module. This programmer is used to upload code to the ESP32-CAM and establish serial communication during development and debugging.

PIR Motion Sensor (HC-SR501)
The Passive Infrared (PIR) motion sensor detects changes in infrared radiation from moving objects, such as humans or animals. When motion is detected, it outputs a high signal to the ESP32-CAM, triggering it to capture an image.

LED Indicator
A simple LED is connected to one of the GPIO pins of the ESP32-CAM. It acts as a visual alert—turning ON when motion is detected and OFF otherwise. This helps in debugging and provides an instant indication of motion detection.

Working Principle
Motion Detection
The PIR sensor constantly monitors the surroundings. When motion is detected, it sends a HIGH signal to the ESP32-CAM. The ESP32-CAM receives this signal via a designated GPIO pin.

Image Capture and LED Alert
Upon motion detection, the ESP32-CAM turns ON the LED and captures an image using the OV2640 camera module. This image can either be stored on a microSD card or sent over the network.

Mobile Notification
The captured image is sent to a cloud server or directly to a mobile app (using platforms like Blynk, Telegram Bot API, or Firebase). The user receives a push notification or image alert, allowing for real-time monitoring from anywhere.

LED Reset
After capturing the image and sending the alert, the LED turns OFF until the next motion event.

Conclusion
This project highlights the integration of embedded systems, computer vision, and IoT communication. With simple components, it delivers a functional and scalable home security solution. The ESP32-CAM module, with its built-in camera and Wi-Fi capabilities, makes it ideal for smart surveillance projects. Future enhancements may include video streaming, facial recognition, and cloud-based storage, making the system even more powerful and intelligent.
