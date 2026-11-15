# ICU Patient Monitoring System

## 📌 Project Overview

The **ICU Patient Monitoring System** is an embedded systems-based project designed to monitor important patient health parameters in real time. It collects sensor data, processes the readings using a microcontroller, and transmits the information to a central monitoring node through CAN communication.

The system helps healthcare professionals monitor multiple patient parameters and identify abnormal conditions quickly.

## 🎯 Objectives

- Monitor patient health parameters continuously.
- Collect sensor data using a microcontroller.
- Transfer patient data using CAN communication.
- Display the received information through UART.
- Support centralized monitoring of patients in an ICU environment.

## ⚙️ Hardware Components

- LPC2129 / LPC2138 Microcontroller
- Temperature Sensor
- LDR Sensor
- SpO2 Sensor / Sensor Module
- CAN Transceiver
- UART Communication Interface
- Power Supply

## 💻 Software Tools

- Keil µVision
- Embedded C
- Proteus Design Suite
- UART Serial Terminal

## 🔌 Communication Protocols

### 1. CAN Protocol
CAN communication is used to transfer patient sensor readings between monitoring nodes. It supports reliable communication between multiple embedded devices.

### 2. UART Protocol
UART is used to display the received sensor values on a serial terminal for monitoring and debugging.

## 🏗️ Working Principle

1. Sensors collect patient-related readings.
2. The microcontroller reads the sensor values through its ADC interface.
3. The sensor readings are converted into digital values.
4. The data is packed into a CAN message.
5. The transmitting node sends the CAN message to the receiving node.
6. The receiving microcontroller extracts the individual sensor values.
7. The received values are displayed on the UART terminal.

## 📊 Parameters Monitored

| Parameter | Purpose |
|---|---|
| Temperature | Monitors body temperature |
| LDR | Demonstrates light-level sensing |
| SpO2 | Represents oxygen saturation data |

## 📁 Project Structure

```text
ICU-PATIENT-MONITORING-SYSTEM/
│
├── Node_A/
│   └── Transmitter source files
│
├── Node_B/
│   └── Receiver source files
│
├── Proteus/
│   └── Simulation files
│
├── README.md
└── header.h
```

## 🚀 Applications

- ICU patient monitoring demonstrations
- Embedded healthcare monitoring systems
- Multi-node sensor communication
- CAN-based medical monitoring prototypes

## 🔮 Future Enhancements

- Add a local hospital server for centralized patient monitoring.
- Develop a graphical user interface for displaying patient data.
- Add alarms for abnormal sensor readings.
- Store patient readings in a database.
- Support monitoring of multiple patients simultaneously.

## ⚠️ Disclaimer

This project is an educational prototype for embedded systems and communication learning. It is not a certified medical device and must not be used for clinical diagnosis or treatment.

## 👨‍💻 Author

**B. Hari Prakash**

**Domain:** Embedded Systems  
**Microcontroller:** LPC2129 / LPC2138  
**Programming Language:** Embedded C
