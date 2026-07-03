# RFID Attendance System with Excel Integration

A practical IoT project built using an Arduino Uno and an RFID-RC522 module to track student attendance. The system scans unique card/keychain UIDs and streams the check-in and check-out logs directly into Microsoft Excel via the native Data Streamer add-in.

## 🚀 Features
* **Live Database:** Registers student profiles (Name, Roll Number) using unique RFID hex codes.
* **Smart Toggle Logic:** Automatically alternates student status between `STUDENT ENTERED` and `STUDENT EXITED` on consecutive scans.
* **Real-time Excel Streaming:** Leverages Excel's Microsoft Data Streamer to log clean CSV data instantly into spreadsheet cells without third-party software.
* **Time Tracking:** Employs an internal mathematical clock using `millis()` to stamp exact entry and exit times.

## 🛠️ Hardware Requirements
* Arduino Uno
* RFID-RC522 Sensor Module
* RFID Cards / Keychains (13.56 MHz)
* USB Data Cable & Jumper Wires

## 🔌 Pin Connections
* **SDA (SS)** -> Pin 10
* **SCK** -> Pin 13
* **MOSI** -> Pin 11
* **MISO** -> Pin 12
* **RST** -> Pin 9
* **GND** -> GND
* **3.3V** -> 3.3V *(Warning: Do not connect to 5V)*
