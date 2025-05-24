# Integration-of-Carbon-Footprint-Sensor-with-IoT

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

1. Open Arduino IDE.
2. Instal DFRobot_SCD4X library and use singleShotMeasure.
3. Connect the I2C interface to the Arduino Nano 33 BLE board.
4. Connect the Arduino Nano 33 BLE board to your device.
5. Start taking carbon dioxide readings from different places.
6. Save and arrange your data in Excle sheet.
7. Create an Edge Impulse account.
8. Analyze your data using Edge Impulse after converting your data to an Excel file in CSV (comma-separated value) form.

**Edge Impulse Integration**

1. Log/Sign in to your Edge Impulse account and create a new project.
2. Follow the instructions to add a new data acquisition source and select Arduino as the device type.
3. Configure the data acquisition parameters and collect training data for CO2 level detection.
4. Train your machine learning model using Edge Impulse's built-in tools.
   
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

After testing, the accuracy from the modal testing output shows that we have an accuracy of 94.74%.All data in your test set is classified by the neural network. Items in green are classified correctly and items in red are misclassified.

<img width="687" alt="image" src="https://github.com/user-attachments/assets/eeee7ce3-4b39-45d3-bd83-af8c548bff60" />

After choosing the maximum absolute regression error of 4, and based on the last training, we have a loss of 9.22, and the data explorer has been shown as:

<img width="703" alt="image" src="https://github.com/user-attachments/assets/ee47268d-6b90-45c8-aa72-d385dfa76b88" />

# Acknowledgments:

I extend my thanks to all those who contributed to the success and completion of this project to reach its current results, and we especially thank Dr. Rama Sami, for helping us in providing the tools for this project.

# Conclusion

The Arduino Nano 33 BLE is a choice, for projects due to its compact size and Bluetooth Low Energy (BLE) capability making wireless data transmission effortless for remote monitoring. Incorporating Edge Impulse takes things up a notch by enabling the development of machine learning models to detect CO2 levels enhancing the effectiveness of your monitoring system.

What makes this project stand out is its focus on open source components encouraging experimentation and innovation to devise solutions for sensing and IoT applications. The flexibility allows you to adapt the system for purposes whether its monitoring air quality in areas or tracking wildlife in natural settings.

At its essence this project aims to create interconnected systems that safeguard our surroundings. It represents a significant stride towards achieving objectives such, as sustainability improved health outcomes and responsible resource management.




