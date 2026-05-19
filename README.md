## ⚙️ MCU Data Logger – PCB Design with KiCad  

### 📋 Project Overview

**MCU Data Logger** is a custom PCB that records sensor or system data over time.

It's built around an **ATmega328P‑AU** microcontroller and uses an **EEPROM** (24LC1025) to keep the data even after power is removed. A **DS1337 real‑time clock** timestamps every entry, so you know exactly when something happened.

The board talks to the outside world through **UART, SPI, and I2C** – you can connect it to sensors, displays, or another microcontroller. I also brought out a few spare GPIOs in case you want to add more features later.

The whole design was done in **KiCad** using a **4‑layer stackup** (signal – GND – VCC – signal) to keep noise low and routing tidy.

### 🔧 Key Features

- **4-layer PCB** – Designed and routed in KiCad.
- **ATmega328P-AU** – Main microcontroller for processing and control.
- **💾 24LC1025 EEPROM** – Non‑volatile storage for logged data.
- **⏱️ DS1337 RTC** – Real‑time clock for accurate timestamps.
- **🔌 UART, SPI, I2C** – Multiple communication interfaces.
- **📈 Spare GPIOs** – Brought out for future expansion.

---

## 🔄 Project Flow  

1️⃣ **Microcontroller (ATmega328P-AU)**  
   - Handles all system operations and manages communication.  
   - Reads and writes data to EEPROM for storage.  
   
2️⃣ **RTC Module (DS1337)**  
   - Provides accurate timestamps for logged data.  
   - Communicates via I2C with the MCU.  
   
3️⃣ **EEPROM Storage (24LC1025)**  
   - Stores logged data persistently.  
   - Connected over I2C for data transfer.  

4️⃣ **Communication Interfaces**  
   - **UART**: Serial communication for debugging/logging.  
   - **SPI & I2C**: Expandability for additional peripherals.  

5️⃣ **Power Management & PCB Layout**  
   - Designed for stable operation with proper power routing.  
   - Optimized signal paths to reduce interference and improve reliability.  

--- 

## 🖼️ PCB Design & Visualizations

### 1️⃣ Top Copper Layer
![Top Copper Layer](https://github.com/Tomatto81/MCU_Datalogger/blob/main/images/top_layer.png)

### 2️⃣ Bottom Copper Layer
![Bottom Copper Layer](https://github.com/Tomatto81/MCU_Datalogger/blob/main/images/bot_layer.png)  

### 3️⃣ MCU Datalogger Schematic
![MCU Datalogger Schematic](https://github.com/Tomatto81/MCU_Datalogger/blob/main/images/mcu_datalogger_schematic.svg)  

### 4️⃣ Connectors Schematic
![Connectors Schematic](https://github.com/Tomatto81/MCU_Datalogger/blob/main/images/mcu_datalogger-connectors_schematic.svg)

### 5️⃣ 3D Model (Top & Bottom)
![3D Model - Top](https://github.com/Tomatto81/MCU_Datalogger/blob/main/images/3d_top_layer.png)
![3D Model - Bottom](https://github.com/Tomatto81/MCU_Datalogger/blob/main/images/3d_bot_layer.png)

---

## 📥 Download & Build
The complete project files, including KiCad PCB designs and schematics, are available for download from my **GitHub repository**.

---

## 💬 Feedback & Suggestions
Please feel free to open an **issue** or leave a **comment**.
