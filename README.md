# iotlab5
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
![Image](https://github.com/user-attachments/assets/8ff01bd6-4327-4692-90b5-71d0c7f89981)

4. Mobile App Layout
MIT app interface:

![Image](https://github.com/user-attachments/assets/733f3104-b2cb-43d9-934b-1fb6b20544b1)

URLs that are used for the MIT app inventor:
![Image](https://github.com/user-attachments/assets/df0996c8-4d6a-46f8-a1ec-6a68ebb345a4)


6. Grafana Dashboard 
![Image](https://github.com/user-attachments/assets/3d8523cb-8681-4daa-8434-a460c4979f84)


The Grafana dashboard uses a Time Series panel to display motor speed and commands over time. The panel is connected to InfluxDB, showing how motor speed changes and logging each action in real time. By setting the X-axis to time and the Y-axis to speed (0–100%), the panel provides an overview of motor behavior and system responsiveness.

7. Reflection & Latency
   
During this lab, the mobile app successfully controlled the DC motor via ESP32, and all actions were logged to InfluxDB and displayed on Grafana. The response from the motor had a small delay of about 200–500 ms, mainly due to Wi-Fi network latency and HTTP request processing. Overall, the system worked reliably, but using WebSockets or async code could improve real-time performance. This lab provided valuable experience in integrating hardware, software, and cloud dashboards for IoT control.

#Thonny Terminal:
<img width="950" height="809" alt="image" src="https://github.com/user-attachments/assets/cd75805e-17fa-4719-a6d5-dbc42cdafe46" />
#Influxdb:
<img width="1063" height="818" alt="image" src="https://github.com/user-attachments/assets/9b2ddd7c-e42b-427d-a7ff-63d67f818079" />

#Motor Control using MIT App Inventor video: 
https://youtube.com/shorts/N0eKwn2-lcY?feature=share

#Real time Grafana Dashboard:
https://youtu.be/AIV7n6Pv2tY

