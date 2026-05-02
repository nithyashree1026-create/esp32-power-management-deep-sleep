## ⚡ Boot Process & Startup Behavior

The ESP32 follows a structured boot process controlled by its internal ROM and external flash memory.

**🔹 Boot Sequence:**

Power-on reset initializes system hardware

Bootloader is executed from internal ROM

Firmware is loaded from external flash

Application execution begins

**🔹 Strapping Pins:**

Certain GPIO pins determine boot mode:

GPIO0 → Flash/Download mode
