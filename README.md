# smart-iot-fan-control-system
An IoT-based smart fan control system using ESP32-WROOM, DHT22, PIR sensor, PWM and Supabase for real-time monitoring, automatic temperature-based operation and remote manual fan speed control.
#Project Overview
The Smart IoT Fan Control System is an IoT-based automation project designed to monitor environmental conditions and control fan operation using an ESP32-WROOM microcontroller.

The system integrates a DHT22 temperature and humidity sensor and a PIR motion sensor to enable automatic fan operation. It also provides manual fan control through a Supabase cloud database, allowing users to remotely switch the fan ON/OFF and adjust its speed.

# Objectives

Automate fan operation based on temperature and motion detection.

Monitor real-time temperature and humidity.

Provide remote manual fan control.

Enable variable fan speed using PWM.

Store sensor readings in a cloud database.

# Hardware Components

ESP32-WROOM

DHT22 Temperature and Humidity Sensor

PIR Motion Sensor

DC Fan

MOSFET / Motor Driver

External Power Supply

Connecting Wires

# Software and Technologies

Arduino IDE

Embedded C/C++

Supabase

Wi-Fi Communication

ArduinoJson Library

PWM Control

Working Principle

1. Sensor Monitoring

The DHT22 sensor measures temperature and humidity, while the PIR sensor detects human motion.

2. Automatic Mode

In automatic mode, the PIR sensor toggles the fan ON/OFF upon successive motion detections. When enabled, fan speed is selected according to the measured temperature.

3. Manual Mode

In manual mode, users can control the fan ON/OFF state and set the desired fan speed from 0% to 100% through Supabase.

4. Cloud Integration

The ESP32 communicates with Supabase through Wi-Fi. Sensor readings are uploaded to the database, while fan-control settings are retrieved from the cloud.

5. PWM Fan Speed Control

The ESP32 generates a PWM signal to control the speed of the DC fan through a suitable motor driver.

Supabase Database

# fan_control

id

mode

fan_speed

manual_fan_on

# sensor_data

temperature

humidity

pir

fan_speed

created_at

# Features

Automatic and manual operating modes

Motion-based fan ON/OFF control

Temperature-based automatic speed adjustment

Remote fan speed adjustment

Real-time sensor data monitoring

Cloud-based sensor data storage

# Future Scope

Development of a dedicated web/mobile dashboard

Implementation of a refined fuzzy logic controller

Historical sensor data visualization

Energy consumption monitoring

Improved security and authentication

# Project Status

Hardware and firmware integration with Supabase-based monitoring and control.


