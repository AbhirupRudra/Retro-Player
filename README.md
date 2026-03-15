# 🎵 Retro Player

**Retro Player** is a compact DIY MP3 music player built using an **Arduino Nano**, **DFPlayer Mini**, and a **128×64 OLED display**.
It features a centered retro-style interface with animated waveform visualization and tactile button controls. Music is played directly from a microSD card using the DFPlayer Mini.

The project focuses on **clean embedded UI design using the U8g2 graphics library and custom fonts**.

---

# 📺 Project Demo

Watch the demonstration on YouTube:

🔗 **YouTube Video:**
`Link`

---

# ✨ Features

* 🎶 Standalone MP3 player using **DFPlayer Mini**
* 🖥️ Clean **centered OLED UI**
* 📊 Animated **waveform visualizer**
* ▶️ **Play / Pause control**
* ⏮️ **Next / Previous track buttons**
* 🎨 UI rendered with **U8g2 graphics library and fonts**
* ⚡ Lightweight firmware optimized for **Arduino Nano**
* 🧩 Easy to build and customize

---

# 🧰 Hardware Components

| Component                 | Quantity |
| ------------------------- | -------- |
| Arduino Nano              | 1        |
| DFPlayer Mini             | 1        |
| SSD1306 128×64 OLED (I2C) | 1        |
| Push Buttons              | 3        |
| 8Ω Speaker                | 1        |
| MicroSD Card              | 1        |
| Resistors (1kΩ, 2kΩ)      | 1 each   |
| Breadboard / PCB          | Optional |

---

# 🔌 Circuit Connections

## DFPlayer Mini → Arduino Nano

| DFPlayer    | Arduino                   |
| ----------- | ------------------------- |
| VCC         | 5V                        |
| GND         | GND                       |
| TX          | D10                       |
| RX          | D11 (via voltage divider) |
| SPK1 / SPK2 | Speaker                   |

---

## OLED Display (I2C)

| OLED | Arduino |
| ---- | ------- |
| VCC  | 5V      |
| GND  | GND     |
| SDA  | A4      |
| SCL  | A5      |

---

## Push Buttons

| Function       | Arduino Pin |
| -------------- | ----------- |
| Play / Pause   | D2          |
| Next Track     | D3          |
| Previous Track | D4          |

Buttons use **INPUT_PULLUP**, so the other terminal of each button connects to **GND**.

---

# 💾 SD Card Setup

Format the SD card as **FAT32**.

Create the following structure:

```
/01
   001.mp3
   002.mp3
   003.mp3
```

Tracks will play sequentially.

---

# 📦 Required Arduino Libraries

Install these from the Arduino Library Manager:

* **DFRobotDFPlayerMini**
* **U8g2**

The **U8g2 library** is used for rendering the UI, fonts, and waveform animation on the OLED display.

---

# 🚀 Getting Started

1. Clone the repository

```
git clone https://github.com/yourusername/retro-player.git
```

2. Open the project in **Arduino IDE**

3. Install the required libraries

4. Upload the code to the **Arduino Nano**

5. Insert the microSD card with music files

6. Power the device

Your **Retro Player** will start playing music.

---

# 🎮 Controls

| Button        | Action                              |
| ------------- | ----------------------------------- |
| Play / Pause  | Toggle playback                     |
| Right         | To jump selection to the next icon  |
| Previous      | To jump selection to the next icon  |

---

# 🖥️ OLED Interface

The OLED display shows:

* Project title **Retro Player**
* Current track number
* Play / pause state
* Animated waveform visualizer
* Decorative music icon

The interface is designed to look like a **minimal retro digital music player**.

---

# 🛠 Possible Improvements

* Track progress bar
* Song title scrolling
* Rotary encoder navigation
* Bluetooth audio support
* Rechargeable battery power
* 3D printed portable enclosure

---

# 🎯 Project Goal

Retro Player demonstrates how simple embedded hardware can create a **polished standalone audio device with a graphical UI**, making it a great learning project for:

* Arduino programming
* Embedded graphics using **U8g2**
* Audio module integration
* Hardware interfacing

---

# 🤝 Contributing

Contributions and improvements are welcome.
Feel free to submit **issues, ideas, or pull requests**.

---

# 📜 License

This project is open-source and released under the **MIT License**.

---

⭐ If you like this project, consider **starring the repository**.
