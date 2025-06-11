# AIR-QUALITY-AND-PURITY-MONITORING-DEVICE-USING-ESP8266-MICROCONTROLLER-WITH-BLYNKIT-IOT-CLOUD
An IoT-based Air Purity Monitoring System using ESP8266 and Blynk IoT Cloud. This project measures air quality using the MQ135 sensor and environmental data with the DHT11 sensor. The ESP8266 sends real-time data to the Blynk cloud platform, allowing remote monitoring through a mobile app. It can also trigger alerts or activate devices 
----------------------------------------------------------------------ASPHANTOM19--------------------------------------------------------------------------------------
# 🌬️ Air Purity Monitoring Device using ESP8266 & Blynk IoT

📦 Features
🚦 Real-time Air Quality Monitoring (MQ135)

🌡️ Temperature and Humidity Tracking (DHT11)

📲 Remote Monitoring via Blynk IoT Cloud

🖥️ Live Data Display on 1.96" OLED Screen

💡 Alert System for Poor Air Quality

🔌 Low-cost and IoT-enabled Smart Device

🧰 Components Used
| Component                           | Description                              |
| ----------------------------------- | ---------------------------------------- |
| ESP8266 (NodeMCU)                   | Wi-Fi enabled microcontroller            |
| MQ135                               | Air quality sensor (CO₂, NH₃, NOx, etc.) |
| DHT11                               | Temperature & humidity sensor            |
| 1.96" OLED Display                  | SPI/I2C OLED for live data               |
| Resistors, Breadboard, Jumper wires | Basic electronics accessories            |


🔗 Circuit Diagram
MQ135 → A0 (analog) on ESP8266

DHT11 → Digital pin (D4 or D2)

OLED (SPI/I2C) → SDA/SCL → D2/D1 or based on your model

3.3V and GND to power the sensors
![Screenshot 2025-06-11 173058](https://github.com/user-attachments/assets/45a1d286-14d5-4c81-9adf-cee0e61873dc)


🔧 How It Works
*MQ135 detects air pollutants and sends analog data.

*DHT11 captures temperature & humidity.

*ESP8266 processes the sensor data.

*OLED displays the data locally.

*Blynk IoT Cloud receives the data via Wi-Fi.

*The Blynk app/web dashboard lets users see real-time air quality remotely.

📱** Blynk Configuration**

*Sign up on Blynk IoT Cloud

*Create a new Template and Device

*Add virtual pins for:

*V0: Air Quality

*V1: Temperature

*V2: Humidity

*Get your Auth Token from the Blynk dashboard

*Replace the token in your Arduino code

🧠 Code Overview

*Arduino code includes:

*MQ135 analog value reading

*DHT11 sensor data using the DHT.h library

*OLED display using Adafruit_SSD1306 or U8g2

*Blynk communication via BlynkSimpleEsp8266.h

**Remember to install all required libraries via Arduino Library Manager.

🚀 **Future Improvements**

*Add PM2.5/PM10 dust sensors (e.g., PMS5003)

*Enable data logging to SD card or Google Sheets

*Integrate buzzer or LED warning system

*Add auto air purifier trigger

📸 Preview
(Upload screenshots of Blynk dashboard and OLED display here)
Example OLED Output:



Air Quality: 172

Temp: 28.5°C

Humidity: 65%
🧪 **Applications**
*Indoor Air Quality Monitoring
*Smart Home Automation
*IoT Learning Projects
*Health & Safety Devices

