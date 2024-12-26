 Automatic-Plant-Watering-System-System
This project is an Automatic Plant Watering System that uses an Arduino, a soil moisture sensor, and a relay module to automate the watering process for plants. It monitors the soil moisture levels, controls a motor (water pump) based on the moisture readings, and displays the status on an LCD screen. The system will turn the motor on or off depending on whether the soil is dry, humid, or wet.

Components Used:
Arduino (Uno or compatible): The microcontroller that controls the system.
Soil Moisture Sensor: Reads the moisture level of the soil.
Relay Module: Used to control the water pump (motor) based on sensor input.
LCD Display (16x2 with I2C): Displays the soil moisture level and the motor status.
Water Pump (optional): Controlled by the relay to water the plant if the soil is dry.
Features:
Soil Moisture Detection: The system reads the analog value from the soil moisture sensor to determine whether the soil is dry, medium, or wet.
Motor Control: The water pump is activated when the soil is dry and deactivated when it is wet or has medium moisture.
LCD Display: The moisture status and motor status are displayed on the LCD screen for easy monitoring.
Serial Monitor: Soil moisture values and status messages are printed to the serial monitor for debugging and analysis.
How It Works:
Sensor Reading: The soil moisture sensor is connected to the analog pin (A0). The Arduino reads the moisture level and converts it into a digital value.
Motor Control: Based on the moisture level:
If the soil is dry (sensor value > 600), the motor is turned on.
If the soil is medium (sensor value between 370 and 600), the motor is turned off.
If the soil is wet (sensor value < 370), the motor is turned off.
LCD Display: The soil moisture status and motor status are shown on the LCD screen.
Serial Monitor: The system prints the moisture level and its corresponding status on the serial monitor for monitoring.
