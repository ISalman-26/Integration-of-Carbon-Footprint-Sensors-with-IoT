# Integration-of-Carbon-Footprint-Sensors-with-IoT
Carbon FootPrint Sensor

Done by:

Salman Albu Shaqraa 

Mohammed Albalam 

# Overview 

This project demonstrates how to interface a carbon dioxide (CO2) sensor with an Arduino Nano BLE 33 using the I2C communication protocol. The CO2 sensor used in this project provides accurate readings of carbon dioxide levels in the surrounding environment, making it suitable for various applications such as indoor air quality monitoring and more.

# Requirements

Arduino Nano BLE 33 board

Carbon dioxide sensor with I2C interface

Jumper wires

Arduino IDE

Edge Impulse

# Implementation

Open Arduino IDE.
Inatal DFRobot_SCD4X library and use singleShotMeasure.
Connect the I2C interface to the Arduino Nano 33 BLE board.
Connect the Arduino Nano 33 BLE board to your device.
Start taking carbon dioxide readings from different places.
Save and arrange your data in Excle sheet.
Create an Edge Impulse account.
Analyze your data using Edge Impulse after converting your data to an Excel file in CSV (comma-separated value) form.

Edge Impulse Integration

Log/Sign in to your Edge Impulse account and create a new project.
Follow the instructions to add a new data acquisition source and select Arduino as the device type.
Configure the data acquisition parameters and collect training data for CO2 level detection.
Train your machine learning model using Edge Impulse's built-in tools.
# Opservations & Results

We took readings of carbon dioxide from various locations in the city of Al-Ahsa (Kingdom of Saudi Arabia) and at different times and days. We faced some difficulties in moving from one place to another to collect readings during hot weather conditions. Finally, we took readings from different places that were classified in :

(1) as College of Business.

(2) as College of Engineering.

(3) as CCSIT Department.

(4) as Deanship of Student (outdoor).

(5) as Deanship of Student (indoor).

(6) as Kitchen (not at cooking time).

(7) as Living Room.

(8) as Near to Small Garden.

(9) as PYD Department.

And after an estimated 7 minutes of training the flatten block has produce a results shown in the bellow figure:

<img width="681" alt="image" src="https://github.com/user-attachments/assets/82fe656e-dd3a-4d1c-b3f0-aba3fd6d5615" />
