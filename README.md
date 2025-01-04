#Passenger Counting System
This repository contains the codebase for a Passenger Counting System designed to count and display the number of passengers using two distinct approaches:
Staircase Carpet System
Visual Input System

Contents
1. Code_for_ESP
The Code_for_ESP folder contains the Arduino code responsible for the Staircase Carpet System, which:
Uses Force Sensitive Resistor (FSR) sensors to detect foot pressure on the staircase.
Updates and manages the count variables in real-time.
Sends the count data to a web interface for remote monitoring.
Displays the count on an onboard display (e.g., OLED or LCD).
This approach focuses on sensor-based detection for accurate passenger counting.

2. Count_from_CV
The Count_from_CV folder contains the code for the Visual Input System, which:
Processes video streams to detect and count passengers using Computer Vision (CV).
Utilizes OpenCV and YOLO for image processing and people detection.
Passes the computed count variables to the ESP system (via wireless communication).
Synchronizes the CV-based count with the sensor-based count to ensure consistent and accurate updates.
This approach leverages visual data for passenger counting.

Workflow Overview
The Staircase Carpet System utilizes FSR sensors to detect foot pressure and updates the passenger count.
The Visual Input System uses video feeds to count passengers through CV algorithms.
The count values from the Visual Input System are passed to the ESP system to synchronize with the sensor-based count.
Both approaches update a web interface and an onboard display, providing real-time passenger data.

Usage Instructions
Clone this repository.
Choose the appropriate folder based on your desired approach:
Use Code_for_ESP for the Staircase Carpet System.
Use Count_from_CV for the Visual Input System.

Follow the setup instructions provided in each folder to configure hardware and software dependencies.

Hardware Requirements:
ESP microcontroller (e.g., ESP32 or ESP8266)
FSR sensors (for Staircase Carpet System)
Onboard display (OLED/LCD)
Camera module (for Visual Input System)

Software Dependencies:
Arduino IDE (for ESP programming)
Python (for Visual Input System)

Contributions are welcome! If you have ideas or suggestions, feel free to submit issues or pull requests to enhance the system.
