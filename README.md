# EcoShield
An integrated IoT framework designed for smart infrastructure that harmonizes advanced security with adaptive power consumption

EcoShield is an Arduino-based IoT solution that integrates multi-factor authentication, intrusion detection, and occupancy-aware energy optimization into a single, cohesive smart-building framework.

## 🚀 Key Features
- **Multi-Layer Authentication:** Dual-stage verification using EM-18 RFID and a 4x4 Matrix Keypad.
- **Adaptive Energy Management:** Real-time occupancy detection via Ultrasonic sensors to toggle electrical loads, reducing energy waste.
- **Advanced Security Suite:** - Intrusion detection using IR sensors.
    - Tamper-proofing with Tilt sensors.
    - Time-restricted access via DS3231 RTC.
- **Remote Monitoring:** GSM-enabled alerts for security breaches and system status.

## 🛠️ Hardware Requirements
- **Microcontroller:** Arduino Mega 2560
- **RFID Reader:** EM-18 Module (125kHz)
- **Input:** 4x4 Membrane Keypad
- **Sensors:** HC-SR04 (Ultrasonic), IR Obstacle Sensor, SW-520D (Tilt)
- **Clock:** DS3231 I2C RTC Module
- **Output:** 16x2 I2C LCD, 5V Relay Module, Active Buzzer

## 📂 Circuit Connectivity
| Component | Arduino Mega Pin | Interface |
|-----------|------------------|-----------|
| EM-18 TX  | Pin 19 (RX1)     | Serial    |
| Keypad    | Pins 22-29       | Digital   |
| RTC (SDA) | Pin 20           | I2C       |
| RTC (SCL) | Pin 21           | I2C       |
| IR Sensor | Pin 2            | Interrupt |
| Relay     | Pin 11           | Digital   |

## 💻 Software Setup
1. Clone the repository: `git clone https://github.com/yourusername/AegisNode.git`
2. Install the following libraries in the Arduino IDE:
   - `Keypad` by Mark Stanley
   - `RTClib` by Adafruit
   - `LiquidCrystal_I2C`
3. Upload `AegisNode.ino` to your Arduino Mega.

## 📜 License
This project is for educational and research purposes.
