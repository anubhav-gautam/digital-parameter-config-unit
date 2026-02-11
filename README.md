# Arduino UNO R4 \- OLED Example

## Overview
Simple example that initializes an SSD1306 I2C OLED and prints a few lines. Main source: `src/main.cpp`.

## IDE
- Primary IDE: `CLion` (CLion 2025.3.2 on Windows)

## Using CLion
- Install CLion and configure a toolchain for embedded development (Arduino CLI or PlatformIO).
- Add project folder to CLion.
- Ensure `src/main.cpp` is in the project tree.
- Use CLion Run/Debug configurations to call the upload script or Arduino CLI.

## Codes
- Main file: `src/main.cpp`
- Behavior: initializes I2C OLED (address `0x3C`), prints startup text, and holds display.

## Libraries
- `Adafruit_GFX`
- `Adafruit_SSD1306`
- `Wire` (Arduino I2C)
- Arduino core for UNO R4

Install via Arduino Library Manager, PlatformIO, or include in your build system.

## Dependencies
- Arduino core for `Arduino UNO R4`
- Adafruit libraries (matching compatible versions)
  - Recommended: `Adafruit_GFX` >= 1.x
  - `Adafruit_SSD1306` compatible with SSD1306 displays
- Arduino CLI or PlatformIO (for command line build/upload)

## Components used with OLED
- `Arduino UNO R4` (or compatible board)
- SSD1306 I2C OLED display (128x64)
- Jumper wires and optional breadboard
- Connections:
  - OLED VCC -> 5V (or 3.3V if required by module)
  - OLED GND -> GND
  - OLED SDA -> SDA pin on UNO R4
  - OLED SCL -> SCL pin on UNO R4
- I2C address commonly `0x3C` (verify with scanner)

## Software Requirements
- Operating System: Windows
- IDE: `CLion` 2025.3.2
- Arduino CLI or Arduino IDE (for board packages / upload)
- Required libraries installed in the Arduino/PlatformIO library path

## Hardware Requirements
- `Arduino UNO R4` board
- SSD1306 I2C OLED display (128x64)
- USB cable to connect board to PC
- Jumper wires / breadboard
- Power supply via USB or external (as needed)

## Author
- `anubhav-gautam` (GitHub account)

## Notes
- Verify the OLED I2C address before `display.begin(...)`.
- Use correct voltage for your OLED module to avoid damage.
