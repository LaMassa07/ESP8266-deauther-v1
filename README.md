# ESP8266-deauther-v1
ESP8266 NodeMcu LoLin v3 DEAUTHER with OLED interface

# Schematic
- ESP8266 NodeMcu LoLin v3 board
- I2C OLED display, 0.96', SSH1306
- 3x buttons
- 3x 220Ω resistors
- RGB common K led
<img width="1416" height="702" alt="image" src="https://github.com/user-attachments/assets/7fc2aff0-62d7-428f-89fd-22e3730b37b7" />

# Code
- download the `CODE` folder, open the `.ino` file
- to change settings, go to the `A_config.h`

## Board
Add `https://arduino.esp8266.com/stable/package_esp8266com_index.json` in the Additional Boards Manager URLs, under "Preferences"
Than, select your COM port and `NodeMCU 1.0 (ESP-12E module)`

## Important upload settings
Upload Speed: "115200"
Flash Size: "4MB (FS:3MB OTA:~512KB)"
Erase Flash: "All Flash Content"
