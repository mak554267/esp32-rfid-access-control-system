# IoT-Based Smart RFID User Management and Access Control System Using ESP32

> A smart IoT-based RFID authentication and access control system built using ESP32, RC522 RFID module, OLED display, SD card logging, LED indicators, buzzer alerts, and a web dashboard for real-time user management and monitoring.

---

## 📌 Features

- 🔐 RFID-based authentication system
- 🌐 Web dashboard using ESP32 Async Web Server
- 💾 SD card logging and persistent storage
- 📟 OLED display for real-time status updates
- 🔔 Buzzer alert system
- 💡 LED indication system
- 📡 WiFi-enabled monitoring
- 🧾 User role management
- 🕒 Real-time date and time display
- 📂 LittleFS filesystem integration
- ⚡ Dual SPI architecture (VSPI + HSPI)

---

## 🛠 Hardware Used

| Component | Description |
|---|---|
| ESP32-WROOM-32D | Main microcontroller |
| RC522 RFID Module | RFID reader |
| SSD1306 OLED | OLED display |
| SD Card Module | Data logging |
| Active Buzzer | Audio alerts |
| LED + 220Ω Resistor | Visual indication |
| RFID Tags/Cards | Authentication |

---

## 🔌 Final Connections

### 📟 RC522 RFID Module (VSPI)

| RC522 Pin | ESP32 Pin |
|---|---|
| SDA / SS | GPIO 5 |
| SCK | GPIO 18 |
| MOSI | GPIO 23 |
| MISO | GPIO 19 |
| RST | GPIO 27 |
| 3.3V | 3.3V |
| GND | GND |

---

### 💾 SD Card Module (HSPI)

| SD Pin | ESP32 Pin |
|---|---|
| CS | GPIO 16 |
| SCK | GPIO 14 |
| MOSI | GPIO 13 |
| MISO | GPIO 25 |
| VCC | 5V |
| GND | GND |

---

### 💡 LED

| LED Part | ESP32 Pin |
|---|---|
| Long Leg (+) | GPIO 26 through 220Ω resistor |
| Short Leg (-) | GND |

---

### 🔔 Active Buzzer

| Buzzer Pin | ESP32 Pin |
|---|---|
| Long Leg (+) | GPIO 4 |
| Short Leg (-) | GND |

---

### 📟 OLED Display (I2C)

| OLED Pin | ESP32 Pin |
|---|---|
| VCC | 3.3V |
| GND | GND |
| SDA | GPIO 21 |
| SCL | GPIO 22 |

---

## 📷 OLED Features

- Access Granted / Denied screen
- RFID UID display
- User role display
- Real-time date & time
- System ready screen

---

## 🌐 Web Dashboard Features

- User management
- Full access logs
- RFID monitoring
- Add/remove users
- Live authentication status

---

## 📚 Libraries Used

- MFRC522
- ESPAsyncWebServer
- AsyncTCP
- Adafruit SSD1306
- Adafruit GFX
- SD
- SPI
- WiFi
- LittleFS

---

## ⚙️ Technical Challenges Solved

- SPI bus conflict resolution
- Dual SPI implementation using VSPI and HSPI
- LittleFS web filesystem integration
- ESP32 boot pin debugging
- SD card communication stabilization
- OLED and RFID synchronization

---

## 🚀 Future Enhancements

- Servo-based smart door lock
- Firebase cloud integration
- Telegram notifications
- Mobile application
- Fingerprint authentication
- Face recognition
- Blockchain-based tamper-proof logs

---

## 📸 Project Demo

### RFID Authentication Flow

```text
RFID Card
   ↓
ESP32 Reads UID
   ↓
OLED Displays Status
   ↓
LED & Buzzer Activate
   ↓
Data Logged To SD Card
   ↓
Web Dashboard Updates
```

---

## 👨‍💻 Author

**Muhammad Azfar Waqas**  
BS Cybersecurity — University of Wah

---

## ⭐ If You Like This Project

Give this repository a ⭐ and share it with others!
