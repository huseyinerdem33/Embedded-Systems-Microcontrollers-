
# 🤖 Embedded Systems & Microcontrollers Ecosystem

Welcome to the ultimate hardware development and firmware engineering repository. This ecosystem is designed as a comprehensive, production-ready blueprint that bridges the gap between low-level hardware computing and high-level system automation. 

Inside, you will find optimized source code, peripheral interfacing schematics, and clean software architectures spanning from bare-metal microcontrollers to advanced single-board Linux platforms. This project focuses heavily on asynchronous execution, wireless IoT telemetry pipelines, and maximizing hardware efficiency across multiple architectures.

---

## 🔌 Supported Platforms & Board Variants

### ⚡ Arduino Family
Arduino remains the global standard for rapid prototyping and core electronics development. Operating primarily on 8-bit AVR architecture, it is ideal for deterministic, real-time sensor loops where operating system overhead is not wanted.
*   **Arduino Uno:** The industry-standard entry board, built around the ATmega328P. Excellent for basic GPIO manipulation and learning hardware timers.
*   **Arduino Nano:** A breadboard-friendly, miniaturized version of the Uno with identical processing power but a much smaller footprint.
*   **Arduino Mega 2560:** Designed for complex projects, offering expanded memory and a massive array of 54 digital I/O pins and 4 UART ports.

<table align="center" border="0" cellpadding="0" cellspacing="0">
  <tr valign="middle">
    <td align="center" style="padding: 10px;">
      <img src="https://github.com/user-attachments/assets/d37c0b82-4895-4991-84cf-72309e64826c" width="220" alt="Arduino Uno">
    </td>
    <td align="center" style="padding: 10px;">
      <img src="https://github.com/user-attachments/assets/ea662528-2604-4175-9ef3-ed51a1c98719" width="160" alt="Arduino Nano">
    </td>
    <td align="center" style="padding: 10px;">
      <img src="https://github.com/user-attachments/assets/e0229ce7-b614-490d-9151-25d190e9d75a" width="310" alt="Arduino Mega">
    </td>
  </tr>
</table>

### 🛡️ ESP32 & ESP8266 (Espressif Systems)
The go-to ecosystem for Internet of Things (IoT) applications. These boards bring massive processing power, dual-core architectures, and native wireless stacks at an incredibly low cost.
*   **ESP8266 (NodeMCU):** The pioneer of low-cost Wi-Fi connectivity. Ideal for simple smart-home nodes and wireless data logging.
*   **ESP32 (WROOM / WROVER):** A powerhouse featuring a dual-core 32-bit processor, native Wi-Fi, Bluetooth Low Energy (BLE), and hardware encryption engines for secure cloud telemetry (MQTT, HTTPS).

<table align="center" border="0" cellpadding="0" cellspacing="0">
  <tr valign="middle">
    <!-- 1. Fotoğraf: ESP32 -->
    <td align="center" style="padding: 15px;">
      <img src="https://github.com/user-attachments/assets/c34fdf7a-55c9-40b3-9c39-688ed912c0fc" width="280" alt="ESP32 DevKitC">
    </td>
    <!-- 2. Fotoğraf: ESP8266 NodeMCU -->
    <td align="center" style="padding: 15px;">
      <img src="https://github.com/user-attachments/assets/f129e1be-868f-42af-8a48-6b94a2adf760" width="280" alt="ESP8266 NodeMCU">
    </td>
  </tr>
</table>

### 🔄 STM32 (STMicroelectronics)
An industry-grade platform based on the powerful **ARM Cortex-M** architecture. STM32 boards are heavily used in automotive, medical, and industrial automation due to their safety-critical design and extreme clock speeds.
*   **STM32 Blue Pill (F103C8T6):** The most popular budget ARM board, offering 72MHz speeds, Direct Memory Access (DMA), and true hardware USB support.
*   **STM32 Nucleo Series:** Official development boards from ST, featuring onboard ST-LINK debuggers, Arduino shield compatibility, and advanced power management.

 *[<img width="250" height="540" alt="R1939784-01" src="https://github.com/user-attachments/assets/9e81390d-489d-4758-94ef-977275304907" />]*

---

### 💻 Raspberry Pi Series
Unlike the previous microcontrollers, Raspberry Pi boards are true **Single Board Computers (SBC)** that run full Linux-based operating systems. They are designed for heavy computational tasks, Edge AI processing, and high-level network gateway scripting.
*   **Raspberry Pi 4 / 5:** Full desktop-class computers with quad-core processors, dual 4K display outputs, Gigabit Ethernet, and up to 8GB/16GB of RAM.
*   **Raspberry Pi Zero W / 2 W:** Ultra-small, low-power Linux boards with built-in Wi-Fi, perfect for embedded camera servers and minimal background scripts.

📸 *[Drop your Raspberry Pi family hardware image here]*

---

## 🛠️ Software Setup & Environment Configuration

To program the Arduino, ESP32, and STM32 boards within this repository, we use the **Arduino IDE** environment. Follow the guide below to set up your workstation.

<details>
<summary><b>➔ 🛠️ Click here for Step-by-Step Arduino IDE Installation Guide</b></summary>
<br>

### 1. Download the Installer
Go to the official [Arduino Software Center](https://www.arduino.cc/en/software) and download the latest version of Arduino IDE for your operating system (Windows, macOS, or Linux).
<br>
📂 *[Drop / Paste Step 1 Download Page Screenshot Here]*
<br><br>

### 2. Run the Setup Wizard
Launch the downloaded installer. Accept the license agreement, leave the default components checked (especially the USB driver options), and select your installation directory.
<br>
📂 *[Drop / Paste Step 2 Installation Wizard Screenshot Here]*
<br><br>

### 3. Installing Third-Party Boards (ESP32 & STM32)
By default, the IDE only supports Arduino boards. To add ESP and STM boards:
1. Open Arduino IDE and go to `File` > `Preferences`.
2. Locate the **Additional Boards Manager URLs** field and paste the required URLs:
   * **ESP32:** `https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json`
   * **STM32:** `https://github.com/stm32duino/BoardManagerFiles/raw/main/package_stmicroelectronics_index.json`
3. Go to `Tools` > `Board` > `Boards Manager...`, search for **ESP32** or **STM32**, and click **Install**.
<br>
📂 *[Drop / Paste Step 3 Preferences & Boards Manager Screenshot Here]*

</details>

---
