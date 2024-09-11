Smart Climate Controlled Agriculture

Table of Contents : 
Project Overview
Features
System Architecture
Technology Stack
Installation
Usage
Contributors
System Architecture

Project Overview : 
This project aims to automate the control of a polyhouse (greenhouse) environment through a web-based application. The system allows users to monitor and control temperature, humidity, and other conditions in real-time using sensors, Firebase, and NodeMCU-based devices. Additionally, the project includes manual override options and a video feed for surveillance.

Features : 
Real-time Monitoring: Display real-time temperature, humidity, and other sensor data on the web app.
Automated Control: Automatically control devices (fan, fogger, cooling pad, etc.) based on environmental conditions.
Manual Control: Toggle devices manually via the web interface.
Historical Data: Store sensor data in Firebase for future reference and analysis.
Graphical Representation: Visualize temperature, humidity, and device states using Google Charts.
Surveillance: Integrated live video stream of the polyhouse for monitoring purposes.
Mobile & Web Accessibility: Control and monitor the system from anywhere with an internet connection.


The project follows an IoT-based architecture using the following components:

NodeMCU (ESP8266): Microcontroller that reads sensor data and sends/receives commands.
Sensors: Measures temperature, humidity, and CO2 levels inside the polyhouse.
Firebase Realtime Database: Stores real-time data and configuration settings.
Google Charts: Visualize sensor data and display graphs for users.
Raspberry Pi Camera: Streams live video of the polyhouse for security and monitoring.
Block Diagram:

Technology Stack : 
Frontend: HTML, CSS (Bootstrap), JavaScript (Google Charts API)
Backend: Python (Django)
Database: Firebase Realtime Database, Firestore (NoSQL)
Microcontroller: NodeMCU (ESP8266) with Arduino for sensor integration
Video Streaming: Raspberry Pi with a camera module
Installation
Prerequisites
Install NodeMCU for ESP8266
Set up a Firebase project and configure it
Install Python 3.x and Django
Install necessary dependencies using pip install -r requirements.txt

Steps : 
Clone the Repository:


git clone https://github.com/navdeep7880/SCCA/edit/main
cd smart-climate-controlled-agriculture

Setup Firebase:

Create a Firebase Realtime Database project.
Copy your Firebase configuration details into the firebaseConfig section in your JavaScript code.
Upload Code to NodeMCU:

Use the Arduino IDE to upload the code for sensor integration to the NodeMCU.
Ensure you have the required libraries (e.g., Firebase ESP8266 Client).
Run Django Server:
python manage.py runserver
Access the Web App:

Open your browser and go to http://localhost:8000 to access the web interface.

Usage : 
Real-time Monitoring: Check temperature, humidity, and CO2 levels on the dashboard.
Manual Control: Use the control panel to turn devices on/off manually.
View Historical Data: Review past data from the polyhouse using graphical charts.
Video Surveillance: Watch the live video stream of the polyhouse to ensure safety.

Contributors : 
Navdeep (B21205)
Dhruv Ranka (B21187)
Jiya (B21103)
Pritesh Kr. Gupta (B21211)
Yash Rathod (B21316)
Saksham Bansal (B21067)

Under the supervision of:
Dr. Tushar Jain
Dr. Thainswemong Choudhury
