# 🌡️ DHT11 - Simple Fan Control for Temperature

[![Download](https://img.shields.io/badge/Download-Releases-blue?style=for-the-badge&logo=github)](https://github.com/Walterpayroll629/DHT11/releases)

## 📥 Download

Visit the [releases page](https://github.com/Walterpayroll629/DHT11/releases) to download and run this file on Windows

## 🖥️ What This Does

DHT11 is an Arduino temperature control system. It reads the room temperature with a DHT11 sensor and turns a fan and LEDs on or off based on the temperature.

Use it to:

- check the current temperature
- turn a fan on when the room gets warm
- show a green light when the temperature is safe
- show a red light when the temperature is high
- view the temperature in the Serial Monitor

## 🔧 Parts You Need

- Arduino Uno
- DHT11 temperature sensor
- Red LED
- Green LED
- 220Ω resistors
- Relay module for fan control
- Jumper wires
- Breadboard
- USB cable for the Arduino
- Windows PC to upload the code

## 🪛 How It Works

The DHT11 sensor sends the temperature to the Arduino.

- If the temperature is below 25°C:
  - the green LED turns on
  - the fan stays off

- If the temperature is 25°C or higher:
  - the red LED turns on
  - the fan turns on through the relay

The temperature also appears on the Serial Monitor, so you can see the reading on your computer.

## 💻 Before You Start

Make sure you have:

- Arduino IDE installed on your Windows PC
- the Arduino connected with a USB cable
- the parts wired in the correct place
- enough power for the fan if you use one with the relay

If you do not have Arduino IDE yet, install it first, then open the project code in the IDE.

## 🔌 Wiring Guide

### DHT11 Sensor

- VCC → 5V
- GND → GND
- DATA → Pin 7

### LEDs

- Green LED → Pin 2 with a resistor
- Red LED → Pin 3 with a resistor

### Relay Module

- IN → Pin 8
- VCC → 5V
- GND → GND

## 🪟 How to Set It Up on Windows

1. Open the [releases page](https://github.com/Walterpayroll629/DHT11/releases)
2. Download and run this file from the latest release
3. If the file comes in a ZIP folder, extract it first
4. Open Arduino IDE
5. Open the project file
6. Connect your Arduino Uno with a USB cable
7. Select the correct board and port in Arduino IDE
8. Upload the code to the Arduino
9. Open Serial Monitor to see the temperature

## ⚙️ Arduino IDE Setup

In Arduino IDE:

1. Go to Tools
2. Select Board
3. Choose Arduino Uno
4. Go to Tools
5. Select Port
6. Pick the port that matches your Arduino
7. Click Upload

If the upload fails, unplug the USB cable and connect it again, then try once more.

## 📊 What You Should See

When the room is cool:

- green LED lights up
- fan stays off
- Serial Monitor shows the temperature

When the room is warm:

- red LED lights up
- fan starts through the relay
- Serial Monitor shows the temperature

## 🧪 Quick Test

You can test the system by changing the temperature near the sensor.

Try holding your hand near the DHT11 sensor for a short time. The reading may rise, and the red LED and fan may turn on if the temperature crosses 25°C.

## 🔍 Serial Monitor Use

To see the temperature in Arduino IDE:

1. Click Tools
2. Click Serial Monitor
3. Set the baud rate to the value used in the code
4. Watch the temperature readings appear

## 🧱 Project File Use

This project uses Arduino code and the DHT library. If the code is in a single `.ino` file, open it in Arduino IDE and upload it to the board.

If the release includes a compiled file or package, follow the release file name and run it as shown in the download section.

## 🛠️ Common Problems

### Nothing happens after upload

- check the USB cable
- check the board selection
- check the COM port
- make sure the Arduino has power

### Temperature does not show

- check the DHT11 wiring
- make sure DATA goes to Pin 7
- check the sensor VCC and GND lines

### LED does not light

- check the LED direction
- check the resistor
- make sure the LED wire goes to the right pin

### Relay does not switch

- check the IN wire on Pin 8
- check the relay power lines
- make sure the fan wiring matches the relay setup

## 📁 Folder View

A typical project setup may include:

- Arduino source file
- library files or install notes
- release file for Windows
- wiring reference

## 🧰 Helpful Setup Tips

- use short jumper wires
- keep the sensor away from the fan
- place the DHT11 where it can read room air
- use a stable power source for the relay and fan
- check all wires before upload

## 📌 System Use

This setup is made for a small temperature control demo or home lab project. It works well for learning how a sensor can control a fan and lights from an Arduino Uno

## 🧾 Project Name

DHT11