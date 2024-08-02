# Inventory-Management-System
IoT based smart inventory management system is a modern approach to managing inventory that leverages the power of the internet of things (IoT) technology. The system uses a network of interconnected devices, sensors, and software to track inventory levels, monitor product movement, and optimize inventory levels in real- time.
# Inventory Management System

## Overview
The Inventory Management System is a project designed to monitor the stock levels of products using ultrasonic sensors and an ESP8266 microcontroller. This system tracks the quantities of Ice Cream and Chocolate and sends the data to ThingSpeak for remote monitoring.

## Features
- Measures product levels using ultrasonic sensors.
- Updates stock quantities to ThingSpeak.
- Monitors two products: Ice Cream and Chocolate.

## Prerequisites
- ESP8266 microcontroller
- Ultrasonic sensors (HC-SR04 or similar)
- ThingSpeak account and API key
- Wi-Fi network

## Installation
1. **Hardware Setup:**
   - Connect the ultrasonic sensors to the ESP8266 according to the pin configuration:
     - `trigPin` and `echoPin` for Ice Cream
     - `trig1Pin` and `echo1Pin` for Chocolate

2. **Software Setup:**
   - Install the required libraries in the Arduino IDE:
     - `ESP8266WiFi`
     - `WiFiClient`
     - `ThingSpeak`
   - Include these libraries in your sketch.

3. **Configuration:**
   - Replace the placeholders in the code with your actual credentials:
     - `myWriteAPIKey`: Your ThingSpeak write API key
     - `ssid`: Your Wi-Fi network name
     - `pass`: Your Wi-Fi password
     - `myChannelNumber`: Your ThingSpeak channel number

## Usage
1. Upload the code to your ESP8266 using the Arduino IDE.
2. Open the Serial Monitor to view the status messages and product levels.
3. The system will continuously measure the stock levels of Ice Cream and Chocolate and update ThingSpeak with the latest data.

## Output
![Screenshot 2024-08-02 225009](https://github.com/user-attachments/assets/2014dbf9-09c4-49dd-8c44-60220d34f0cb)
![Screenshot 2024-08-02 225024](https://github.com/user-attachments/assets/ce052fa2-e836-4f23-91fc-44f393dc4cdb)

## Notes
- Ensure the ultrasonic sensors are properly calibrated for accurate measurements.
- The system updates the stock levels based on predefined distance thresholds.
- For remote monitoring, check the ThingSpeak dashboard associated with your channel.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
