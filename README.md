# 👶 Baby Monitoring System using Arduino IoT Cloud

A smart IoT-based Baby Monitoring System that collects and streams real-time sensor data to the Arduino IoT Cloud, enabling parents to remotely monitor their baby's safety and environment from anywhere in the world 🌍.

---

## 📌 Features

- 🌡️ **Temperature Monitoring** – Tracks room temperature using the DHT11 sensor.
- 💧 **Humidity Monitoring** – Measures humidity levels for baby comfort.
- 👶 **Motion Detection** – Detects baby's movement using a PIR sensor.
- 🔊 **Sound Detection** – Captures surrounding noise or baby's cry via a sound sensor.
- 🍼 **Moisture Detection** – Uses a soil moisture sensor to detect wet cradle conditions.

---

## 🧠 Objective

To create an affordable, real-time, and remotely accessible solution for baby monitoring using IoT technologies. This system helps parents stay informed and alert, no matter where they are.

---

## 🛠️ Tech Stack

- **Microcontroller**: Arduino Uno  
- **Platform**: Arduino IoT Cloud  
- **Programming Language**: C++ (Arduino Sketch)  
- **Sensors Used**:
  - DHT11 (Temperature & Humidity)
  - PIR Motion Sensor
  - Analog Sound Sensor
  - Soil Moisture Sensor  

---

## 🔗 Arduino IoT Cloud Integration

- Real-time data from all sensors is sent to the **Arduino IoT Cloud Dashboard**.
- Data can be monitored via web or mobile app interfaces.
- ArduinoCloud.begin() establishes secure connection to the dashboard.
- Variables (motion, temperature, humidity, sound, moisture) are declared in `thingProperties.h`.

---

## 📷 Dashboard Preview

<img width="1919" height="849" alt="Screenshot 2024-03-18 232614" src="https://github.com/user-attachments/assets/a5663a26-3e33-4ef0-8421-18c634486576" />


---

## 🧾 Sample Code Snippet

```cpp
float temp = dht.readTemperature();
temperature = temp;

sound = analogRead(sound_sensor);
motion = analogRead(PIR_sensor);
moisture = analogRead(Moisture_sensor);
```

🚀 Future Enhancements
Add camera module for live video feed 📷

Push email or mobile alerts on abnormal sensor values 📩

Improve UI/UX of the monitoring dashboard

📃 License
This project is licensed under the MIT License. Feel free to use and modify for educational purposes.

🙌 Acknowledgements
Thanks to the Arduino IoT Cloud platform and open-source sensor libraries for making this project possible.

📫 Contact
Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/sarvesh-sivasankaran/) or raise an issue for suggestions!

---
