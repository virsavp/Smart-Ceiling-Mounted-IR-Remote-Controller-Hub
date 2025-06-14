Universal Remote Controller Hub


📂 Jump to Files:

🔧 Hardware (schematics & PCB)
💻 Firmware Code (coming soon)



This project is a compact, ceiling-mountable, smart IR controller hub based on the ESP32-S3-WROOM. 
It enables universal control of IR-based appliances like TVs, air conditioners, and fans using web UI, OTA, and automation features.


✨ Features

🔁 360° IR transmission with 10× TSAL6200 high-power IR LEDs
🔍 IR learning using TSOP38238 receiver
📡 Wi-Fi OTA updates + USB flashing via BOOT jumper
🌡️ DS18B20 temperature sensor (for fan/AC automation)
🔊 Optional WS2812 RGB LED status indicator
🖥️ Optional OLED display via JST I²C header (GPIO17/18)
🔘 Single config/setup button (GPIO2, safe boot compliant)
💾 External SPI flash (W25Q256JV) for IR code storage
🔌 USB-C power + LiPo battery with TP4056 charge module
🧲 Magnetic ceiling-mount enclosure with transparent IR window and venting

🧱 Hardware Overview	
	
Component	Details
MCU	- ESP32-S3 WROOM
IR TX	- 10× TSAL6200 + 2N2222 transistor driver
IR RX	- TSOP38238
Temp Sensor	- DS18B20 (GPIO10)
OLED Display	- SSD1306 via I²C (GPIO17=SDA, GPIO18=SCL)
RGB LED	- WS2812-2020 (GPIO16)
Button	- Config input on GPIO2 (1k pull-up)
External Flash	- W25Q256JV (CS: GPIO13, CLK: GPIO15, MOSI: GPIO5, MISO: GPIO4)
Power Input	- USB-C + LiPo via TP4056
Regulator	- AMS1117-3.3

📁 Repository Structure

/hardware/         → KiCad schematics, PCB files (licensed under CERN-OHL-S)
/3d_model/         → Enclosure STL or CAD (licensed under CC BY-SA 4.0)
/code/             → ESP32 firmware (to be added after layout)
LICENSE            → Dual license for hardware and enclosure
README.md          → This file

🧾 License

🔧 Schematics & PCB Design: CERN-OHL-S v2

🚧 Development Status

✅ Hardware design complete✅ PCB layout and routing complete🔲 Firmware development starts after placement confirmation


🙌 Contributions

Feel free to fork, improve, or repurpose this design. If you build upon it, keep it open-source under the same licenses.
For issues or suggestions, please open a GitHub issue or contact the maintainer.


Made with ❤️ by Vishnu – Electronics Hobbyist | KiCad Enthusiast | Open Hardware Advocate
