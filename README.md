LAB5- Mobile App DC Motor Control with Grafana Dashboard
1. Overview
This project demonstrates a complete IoT system where a DC motor is remotely controlled using a mobile app. The mobile app, built with MIT App Inventor, communicates with an ESP32 running MicroPython by HTTP requests to control motor direction (forward, backward, stop) and speed. All motor actions and speed updates are logged to InfluxDB and visualized in real time using a Grafana dashboard. This setup provides hands-on experience integrating hardware, software, and cloud services, while allowing monitoring and analysis of system performance, latency, and reliability.
2. Equipment
ESP32 Dev Board


L298N Motor Driver


DC Motor + Power Supply


Jumper Wires 


Laptop (Thonny IDE)


MIT App Inventor


Grafana Cloud / Local InfluxDB




3. Wiring Diagram
![Image](https://github.com/user-attachments/assets/64d2ec8b-5ae1-4c6c-b343-b097a9e5dc67)

5. Mobile App Layout
MIT app interface:
![Image](https://github.com/user-attachments/assets/6ed2c8f4-fa1e-4753-b2df-cc1f1e413073)

URLs that are used for the MIT app inventor:
![Image](https://github.com/user-attachments/assets/8a9b8974-0cec-4917-8541-933a9c9f3751)


7. Grafana Dashboard Setup
![Image](https://github.com/user-attachments/assets/d3195051-e46c-43d4-834f-6fa0cc0935b6)


The Grafana dashboard uses a Time Series panel to display motor speed and commands over time. The panel is connected to InfluxDB, showing how motor speed changes and logging each action in real time. By setting the X-axis to time and the Y-axis to speed (0–100%), the panel provides an overview of motor behavior and system responsiveness.

7. Reflection & Latency
   
During this lab, the mobile app successfully controlled the DC motor via ESP32, and all actions were logged to InfluxDB and displayed on Grafana. The response from the motor had a small delay of about 200–500 ms, mainly due to Wi-Fi network latency and HTTP request processing. Overall, the system worked reliably, but using WebSockets or async code could improve real-time performance. This lab provided valuable experience in integrating hardware, software, and cloud dashboards for IoT control.
