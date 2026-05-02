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

GPIO2, GPIO15 → Boot configuration

**🔹 Insight:**

Improper configuration of strapping pins can prevent ESP32 from booting correctly, making hardware design critical.

## 🧠 Memory Management & Partitioning

ESP32 uses a flexible memory architecture for efficient resource utilization.

**🔹 Memory Types:**

DRAM → Data storage

IRAM → Instruction execution

RTC Memory → Retained during deep sleep

**🔹 Partition Table:**

Defines how flash memory is divided:

Bootloader

Application firmware

OTA partitions

File system (SPIFFS/LittleFS)
