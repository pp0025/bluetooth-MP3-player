# 🎵✨ **ESP32 Bluetooth MP3 Player**

### *A Wireless Audio Playback System using ESP32 + DFPlayer Mini + OLED Display*

<p align="center">
  <img src="images/mp3-player-cover.jpg" width="420px" />
</p>

---

## 🚀 **Overview**

This project is a compact and fully functional **Bluetooth-controlled MP3 player** built using the **ESP32**, **DFPlayer Mini**, and a **0.96" OLED display**.
Users can control playback using a **smartphone over Bluetooth**, while the OLED display provides real-time playback information.
Physical push-buttons are included as a backup control system, making this design reliable and user-friendly.

---

## ⚙️ **Tech Stack**

| Category               | Tools / Hardware  |
| ---------------------- | ----------------- |
| **Microcontroller**    | ESP32 Dev Module  |
| **Audio Module**       | DFPlayer Mini     |
| **Display**            | OLED 128×64 (I2C) |
| **Wireless Interface** | Serial Bluetooth  |
| **Input**              | Push Buttons      |
| **Development Tool**   | Arduino IDE       |

---

## ⭐ **Features**

* 🎧 Wireless control via **Bluetooth**
* ▶️ Play, Pause, Next, Previous track control
* 🔈 Volume adjustments
* 🖥️ OLED screen showing track status
* 🖲️ Physical buttons for manual navigation
* 🔌 Compact, low-power design

---

## 🔧 **Hardware Components**

* ESP32 Dev Board
* DFPlayer Mini audio module
* Micro SD card (for MP3 files)
* 0.96" I2C OLED Display
* Push Buttons (3–5 pcs)
* Speaker / Amplifier module
* Jumper wires
* Power input module

---

## 🔌 **Circuit Wiring**

Add your wiring diagram inside:
`/circuit-diagrams/wiring-diagram.png`

### Basic Wiring Overview

* ESP32 ↔ DFPlayer Mini (UART)
* ESP32 ↔ OLED (I2C)
* Push-buttons connected to GPIO pins with pull-up/down configuration
* DFPlayer output connected to speaker/amplifier

---

## 🧠 **How It Works**

1. The ESP32 pairs with a smartphone through **Bluetooth**.
2. User sends audio commands via a Bluetooth terminal app.
3. ESP32 interprets commands and forwards them to the DFPlayer Mini.
4. DFPlayer reads MP3 files from a micro SD card and plays audio.
5. The OLED display updates the current status (track info / state).
6. Physical buttons act as backup/manual control options.

---

## 📱 **Supported Bluetooth Commands**

* Play / Pause
* Next Track
* Previous Track
* Volume Up
* Volume Down

Works with any standard **Bluetooth Terminal App**.

---

## 📁 **Project Folder Structure**

```
esp32-bluetooth-mp3-player/
│
├── src/
│   └── main.ino               ← main program file
│
├── circuit-diagrams/
│   └── wiring-diagram.png     ← add your connection diagram
│
├── images/
│   ├── mp3-player-cover.jpg
│   ├── oled-display.jpg
│   └── dfplayer-setup.jpg
│
└── README.md
```

---

## 📚 **Libraries Used**

```
BluetoothSerial
DFRobotDFPlayerMini
Adafruit SSD1306 / GFX
Wire
```

---

## 🔮 **Future Improvements**

* Add playlist mode
* Add Bluetooth name customization UI
* Introduce equalizer presets
* Add battery voltage monitoring
* Add sleep mode for power saving

---

## ❤️ **Developed By**

**Akash Roy**
Embedded & IoT Enthusiast
📧 [aroy50809@gmail.com](mailto:aroy50809@gmail.com)

---

## ⭐ **Support**

If you find this project helpful or inspiring, please ⭐ **star the repository** — it really helps!

