# RaspberryPi Weather Station

This project focuses on creating an IoT-based weather station using the Raspberry Pi Pico and the BME280 sensor to measure environmental parameters such as temperature, humidity, pressure, and altitude. The primary goal is to read these sensor values and display them in real-time on a web interface.

### Key Components:
1. Raspberry Pi Pico: A cost-effective microcontroller board that handles the core processing.
2. BME280 Sensor: A digital sensor capable of measuring temperature, humidity, pressure, and altitude.
3. MicroPython: The programming language used to interface with the hardware and communicate with the sensor.
4. Web Interface: A simple, lightweight web server running on the Pico that serves a webpage displaying sensor readings in real-time.

### Functional Overview:
1. Hardware Setup:
The BME280 sensor is connected to the Raspberry Pi Pico via I2C communication.
The necessary connections for power, ground, SDA, and SCL are made between the Pico and the BME280.

2. MicroPython Programming:
The Raspberry Pi Pico is programmed using MicroPython to interface with the BME280 sensor.
The code periodically reads sensor data (temperature, humidity, pressure, altitude) from the BME280.

3. Web Server on Pico:
A simple web server is hosted on the Pico. Using MicroPython's socket module, the Pico serves an HTML page that updates sensor readings dynamically.
The readings are fetched via HTTP requests and displayed in a user-friendly format.

4. Real-Time Data Visualization:
The web page displays real-time sensor readings in a tabular or graphical format.
The data refreshes at regular intervals (e.g., every 5 seconds) to provide updated environmental information.

![Alt text](https://github.com/csgoteresa/RaspberryPiWeatherStation/blob/main/Weather%20Dashboard.png)
