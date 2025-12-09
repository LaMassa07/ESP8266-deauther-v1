# ESP8266 Deauther v1  
*A compact Wi-Fi packet experimentation interface with OLED UI & physical buttons*  

<p align="center">
  <img src="https://img.shields.io/badge/ESP8266-NodeMCU-blue?logo=espressif&logoColor=white" />
  <img src="https://img.shields.io/badge/Display-OLED%200.96%22-purple?logo=arduino&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Experimental-orange" />
</p>

> ⚠️ **USE THIS ONLY ON NETWORKS YOU OWN OR HAVE EXPLICIT PERMISSION TO TEST.**  
> This project is intended purely for *learning, debugging and local demonstrations* of Wi-Fi packet behavior.

---

## 📌 Quick Overview
- **Microcontroller:** ESP8266 NodeMCU / LoLin v3  
- **Display:** 0.96" OLED I2C (SSD1306 / SH1106)  
- **Controls:** 3 physical buttons  
- **LED:** RGB (common cathode)  
- **Purpose:** Local Wi-Fi deauth and packet-handling demonstration  

---

## ✨ Key Features
- OLED graphical interface  
- Menu navigation with physical buttons  
- RGB LED for visual feedback  
- Dedicated configuration file `A_config.h`  
- Designed for educational Wi-Fi protocol experimentation  

---

## 🧩 Hardware Components

| Component | Quantity |
|----------|----------|
| ESP8266 NodeMCU / LoLin v3 | 1 |
| 0.96" OLED Display (I2C) | 1 |
| Push buttons | 3 |
| 220 Ω resistors | 3 |
| RGB LED (common cathode) | 1 |
| Wires / breadboard / PCB | — |


<p align=center><img src="https://github.com/user-attachments/assets/7fc2aff0-62d7-428f-89fd-22e3730b37b7"/></p>

<p align=center><em>Connection schematic (I2C for OLED, GPIO for buttons and RGB LED)</em></p>

---

## 🚀 Quick Installation (Arduino IDE)

### 1️⃣ Add ESP8266 board package  
**Arduino IDE → File → Preferences → Additional Boards Manager URLs:**  

`https://arduino.esp8266.com/stable/package_esp8266com_index.json`


### 2️⃣ Install the ESP8266 board  
**Tools → Board → Boards Manager → "esp8266"**

### 3️⃣ Select:
- **Board:** `NodeMCU 1.0 (ESP-12E Module)`  
- **Correct COM port**  

---

## ⚙️ Recommended Upload Settings

| Setting | Value |
|--------|-------|
| Upload Speed | `115200` |
| Flash Size | `4MB (FS:3MB OTA:~512KB)` |
| Erase Flash | `All Flash Content` |

> 👍 These settings help prevent filesystem and upload issues on LoLin/NodeMCU boards.

---

## 🛠️ How to Use the Code
1. Download the **`CODE`** folder from the repository  
2. Open the `.ino` file in the Arduino IDE  
3. Review and customize **`A_config.h`**:  
   - SSID  
   - timeouts  
   - button behavior  
   - etc.  
4. Compile and upload to the ESP8266  
5. Use the buttons to navigate the OLED menu  

> 📦 Some libraries (like SSD1306) may be required. The Arduino IDE will prompt you if any are missing.

---

## 🙌 Credits
Inspired by the work of <a href="https://github.com/spacehuhn">**@spacehuhn**</a>, creator of well-known Wi-Fi pentesting and deauther tools.

---
