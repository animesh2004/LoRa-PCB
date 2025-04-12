# LoRa IoT Sensor Device

## Project Overview
This repository contains the design files for a versatile IoT sensor device that utilizes LoRa communication technology. The device integrates temperature/humidity sensing (DHT11), light detection (LDR), and is powered by an ESP32-S3 microcontroller with a battery management system.

## Hardware Components

### Main Modules
1. **LoRa Module (LORA1276-C1-915MHZ)**
   - Long-range wireless communication
   - Integrated with RFM95 transceiver
   - Operates at 915MHz frequency band

2. **Sensors**
   - DHT11 temperature and humidity sensor
   - LDR (Light Dependent Resistor) for ambient light sensing
   - Pull-up resistor network for sensor integration

3. **XIAO ESP32-S3 Microcontroller**
   - Main processing unit
   - Wi-Fi and Bluetooth connectivity
   - Multiple GPIO pins for sensor interfacing
   - Power-efficient design for battery operation

4. **Battery Management**
   - SK-22002-05 battery protection circuit
   - Charging circuit with status indicators
   - Battery level monitoring

5. **User Interface**
   - Slide switch for power control
   - ON/OFF indicators
   - USB connectivity for programming and charging

## Pin Connections

### LoRa Module Connections
- MOSI, MISO, SCK, NSS for SPI communication
- DIO0-DIO5 for interrupt and control signals
- Reset pin for module initialization
- Connected to 3V power supply

### Sensor Connections
- DHT11 data pin connected to GPIO
- LDR with analog output for light level detection
- VCC (3.3V) and GND connections

### Power Management
- Battery connections (BAT+/BAT-) 
- USB power input
- ON/OFF control via slide switch
- Charging circuit with indicator LEDs

## PCB Design Notes
- Single-layer design with minimal jumper wires
- Sectioned layout with functional blocks:
  - LoRa communication
  - Sensors (DHT11 + LDR)
  - Microcontroller
  - Power management/switching

## Software Requirements
- Arduino IDE or PlatformIO for development
- Libraries needed:
  - LoRa library for RFM95 module
  - DHT sensor library
  - ESP32 core libraries

## Getting Started
1. Connect the battery or USB power
2. Upload the firmware using the USB connection
3. Configure the LoRa parameters according to your network requirements
4. Deploy the device in the desired location

## Applications
- Environmental monitoring
- Smart agriculture
- Remote sensing
- IoT data collection
- Weather stations

## License
This project is released under the MIT License.

## Credits
Designed by: animeshhtripathi779
Date: 2023-04-10
