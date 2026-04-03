# 🔐 Access Attendance System (ESP32 + Fingerprint)

## 📌 Overview
The **Access Attendance System** is a secure access control and attendance tracking solution based on biometric fingerprint recognition. Built around the powerful **ESP32 microcontroller**, this system authenticates users, logs attendance in real-time, and manages access to restricted areas.

It is ideal for **companies, schools, laboratories, and clubs** looking to modernize and automate their attendance and access management processes.

---

## 🚀 Features
- 🔑 **Biometric Authentication** using fingerprint sensor  
- 🕒 **Real-time Logging** of date and time for each access  
- 👥 **User Management** with customizable access permissions  
- 🔔 **Visual & Sound Feedback** (LED + buzzer) for access status  
- 📟 **Display Support** (OLED/LCD) for system interaction  
- 🌐 **Wi-Fi Connectivity** for cloud/database synchronization  
- 💾 Optional **Local Storage** via SD card  

---

## 🛠️ Hardware Requirements
- ESP32 Development Board (Wi-Fi enabled)  
- Fingerprint Sensor (e.g., **R307**, **GT-521F32**)  
- OLED or LCD Display *(optional but recommended)*  
- Buzzer  
- LEDs  
- SD Card Module *(optional)*  
- Jumper wires & appropriate power supply  

---

## ⚙️ Software Requirements
- Arduino IDE  
- ESP32 Board Package  

### Required Libraries:
- `Adafruit Fingerprint Sensor Library`  
- `U8g2` (for OLED display)  
- `WiFi.h`  
- `HTTPClient.h`  

---

## 🔧 Installation & Setup

1. **Hardware Connections**
   - Connect all components according to the wiring diagram below.

2. **Arduino Setup**
   - Install Arduino IDE  
   - Add ESP32 board support  

3. **Install Libraries**
   - Install all required libraries listed above via Library Manager  

4. **Configuration**
   - Edit the `config.h` file:
     ```cpp
     #define WIFI_SSID "your_ssid"
     #define WIFI_PASSWORD "your_password"
     ```
   - Configure server/database parameters if needed  

5. **Upload Code**
   - Select the correct ESP32 board and port  
   - Upload the firmware  

---

## 📡 Usage
- Register user fingerprints via the interface (display or serial monitor)  
- When a user scans their fingerprint:
  - The system verifies identity  
  - Logs timestamp (date & time)  
  - Grants or denies access  
- Data can be:
  - Viewed on the display  
  - Sent to a remote server/cloud  

---

## 🔌 Connection Diagram (Simplified)
ESP32
├── Fingerprint Sensor → UART (RX/TX)
├── OLED/LCD → I2C (SDA/SCL)
├── Buzzer → GPIO
└── LED → GPIO


---

## ✅ Advantages
- High security using biometric authentication  
- Eliminates manual attendance errors  
- Real-time monitoring and logging  
- Scalable and easy to integrate into existing systems  

---

## 📈 Future Improvements
- Mobile app integration  
- Web dashboard for analytics  
- Multi-device synchronization  
- RFID + Fingerprint hybrid system  

---

## 👨‍💻 Author
**Mohamed Moncef Amor**  
Embedded Systems & IoT Engineer  

---

## 📄 License
All rights reserved © Mohamed Moncef Amor  
