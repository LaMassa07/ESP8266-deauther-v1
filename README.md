# ESP8266 Deauther v1  <img src="https://img.shields.io/badge/ESP8266-NodeMCU-blue?logo=espressif&logoColor=white"/> <img src="https://img.shields.io/badge/Display-OLED%200.96%22-purple?logo=arduino&logoColor=white"/> <img src="https://img.shields.io/badge/Status-Experimental-orange"/>
A compact WiFi gadget to perform a variety of actions to test 802.11 networks, using an ESP8266 board.


<br>



## 📌 Features
- **Scan** for WiFi networks and clients
- **Create** docents of WiFi networks (beacon flooding)
- **Confuse** WiFi trackers by sending fake probe requests (probe flooding)
- **Disconnect** selected devices by sending deauth packets (deauthentication attack)

<br>



## ⚙️ Setup
- First, be sure to have the <a href="https://www.arduino.cc/en/software/">Arduino IDE</a> at the last version

### Libraries
Go to `Sketch` → `Include Library` → `Manage Library` and install:
- **ArduinoJson** by *Benoit Blanchon* version 5.x.x
- **ESP8266 and ESP32 OLED driver for SSD1306 displays** by *ThingPulse*
### Board
Go to `File` → `Preferences` and add, in the Additional boards manager URLs field: 
```
https://arduino.esp8266.com/stable/package_esp8266com_index.json
```

Than, go to `Tools` → `Boards` → `Boards Manager` and install:
- **esp8266** by *ESP8266 Community*

<br>

## 🛠️ Installing the code
Open the *.ino* file with the IDE.
Before uploading it, go to the file called `A_config.h`. That is the file you can edit to change the pin settings. In particular, you can:
- **choose** the pins for buttons, led and display
- **adjust** the orentation of the display
- **change** the default SSID and PASSWORD for the web interface

<br>

When you are ready, click **Upload**


<br>


## 🔌 Build the circuit
### Materials:
- ESP8266 NodeMCU LoLin v3 board *(or similar, I only tested that board)*
- SSD1306 OLED display
- 4 x buttons
- 3 x 220Ω resistors
- led RGB *(in order to use my PCB, the led must be common K)*


### Schematic
<img width="1434" height="628" alt="image" src="https://github.com/user-attachments/assets/f98355da-3687-4073-8d25-b9c1f8447c7f"/>

<br>
<br>

## 🖥️ Use
> ⚠️ **USE THIS ONLY ON NETWORKS YOU OWN OR HAVE EXPLICIT PERMISSION TO TEST.**  
> This project is intended purely for *learning, debugging and local demonstrations* of Wi-Fi packet behavior

You can use the device in two ways:
- Using the buttons to scroll the displayed menu
- Using the web interface:
    - Connect you phone or pc to the network called `pwned` *(the default password is "deauther")*
    - In your web browser type `192.168.4.1`


<br>

## 🔋 More
Additionally, you can print the PCB, using the `PCB_Gerber.zip` folder, with some online services like <a href="https://jlcpcb.com/">JLPBC</a> or similar


<br>
<br>
<br>

## 🙌 Credits
Inspired by the work of <a href="https://github.com/spacehuhn">**@spacehuhn**</a>, creator of well-known Wi-Fi pentesting and deauther tools.
<br>
Find Me on:
- [![Github](https://img.shields.io/badge/Github-LaMassa07-purple?style=for-the-badge&logo=github)](https://github.com/LaMassa07)

