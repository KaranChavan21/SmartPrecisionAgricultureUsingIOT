# Smart Agriculture System

This project is a smart agriculture system designed to monitor and control the environmental conditions of a crop field. It uses an Arduino to read sensor data, display it on an LCD, and control motors for water, fertilizer, and pesticide dispensing based on predefined thresholds.

## Introduction

Agriculture is a critical industry that can benefit greatly from automation and smart technology. This project aims to create a smart agriculture system that helps in monitoring and controlling various environmental factors such as temperature, moisture, humidity, and nutrient levels (N, P, K). By using this system, farmers can ensure optimal growth conditions for their crops, leading to better yields and more efficient use of resources.

## Components Used

- Arduino
- LCD Display
- Motors for water, fertilizer, and pesticide dispensing
- Sensors for temperature, moisture, and humidity

## Features

- Reads sensor data at regular intervals
- Displays sensor data on an LCD screen
- Controls motors to dispense water, fertilizer, and pesticides based on sensor readings
- Stores sensor data in PROGMEM to save SRAM

## How It Works

1. **Sensor Data Collection**: The Arduino reads data from temperature, moisture, and humidity sensors.
2. **Data Display**: The collected data is displayed on an LCD screen.
3. **Decision Making**: Based on the sensor readings, the system decides whether to activate the motors to dispense water, fertilizer, or pesticides.
4. **Data Storage**: The sensor data is stored in PROGMEM to save SRAM and can be used for further analysis or control logic.

## Project Setup

1. **Hardware Setup**:
    - Connect the sensors, motors, and LCD to the Arduino as per the wiring diagram.
    - Ensure the connections are secure and the components are functioning correctly.

2. **Software Setup**:
    - Clone this repository to your local machine.
    - Open the Arduino IDE and load the provided code.
    - Upload the code to the Arduino.

## Simulation Link

You can view and interact with the simulation of this project on Tinkercad:

[Smart Agriculture System Simulation](https://www.tinkercad.com/things/0jbviodnJaI-smart-agriculture-system-using-iot?sharecode=H2ChFcYeJNnqX35ua5we5ewrLEHBB98N-fh9a8najw0)

## Adding Your Own Data

To add your own sensor data, modify the `sensorData` array in the code. Here is an example with two data points:

```cpp
const SensorData sensorData[] PROGMEM = {
    {0, 0, 21, 56, 55, 54, 51, 265},
    {0, 1, 30, 51, 65, 65, 50, 264},
    // Add the rest of your data here
};
