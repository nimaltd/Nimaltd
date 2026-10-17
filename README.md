# 👋 Hi, I'm Nima Askari

I'm an electronics engineer and embedded systems developer. For more than 20 years I've been writing C for STM32 microcontrollers, and most of that time has gone into one goal: making libraries that are actually easy to use.

I got tired of fighting messy drivers and overcomplicated code, so I started writing my own, cleaning them up, and sharing them with anyone who needs them.

---

### 💡 What I focus on

Lightweight, non-blocking, easy to drop in C libraries for STM32 (HAL and LL), covering storage, communication, sensors and general drivers. The idea is always the same: add the library to your project and have it working in minutes, not days.

That is what the installers below are for: one command puts a library into an STM32, Zephyr, ESP-IDF, Arduino or PlatformIO project. They work with anyone's library, not only mine, once it has an `installer.yml`.

---

### 🧰 stm32-installer

[![PyPI](https://img.shields.io/pypi/v/stm32-installer)](https://pypi.org/project/stm32-installer/)

Installing one of my libraries takes one command. [stm32-installer](https://github.com/nimaltd/stm32-installer) copies the files into your project and adds the library to your CMake, STM32CubeIDE, Keil, IAR or Makefile project, backing up the project file first. Any library it needs comes with it, and an update keeps your settings.

```bash
pip install stm32-installer
stm32-installer nimaltd/stm32-installer-example
```

That one is [stm32-installer-example](https://github.com/nimaltd/stm32-installer-example), a small library made for trying the installer on: it builds in any STM32 project and blinks an LED without `HAL_Delay()`.

Libraries you can install with it:

| Library | Description | Install |
|---|---|---|
| [seq](https://github.com/nimaltd/seq) | Non blocking state sequencer and interrupt task queue for STM32 | `stm32-installer nimaltd/seq` |
| [ee24](https://github.com/nimaltd/ee24) | Driver for 24xx I2C EEPROMs, 24C01 to 24C512, on the STM32 HAL | `stm32-installer nimaltd/ee24` |
| [spif](https://github.com/nimaltd/spif) | Driver for SPI NOR flash, W25Qxx and compatible, on the STM32 HAL | `stm32-installer nimaltd/spif` |
| [osal](https://github.com/nimaltd/osal) | OS abstraction layer for STM32: the same mutex and delay on bare metal, FreeRTOS and ThreadX | `stm32-installer nimaltd/osal` |
| [littlefs](https://github.com/nimaltd/littlefs) | LittleFS by the littlefs project, ready for stm32-installer | `stm32-installer nimaltd/littlefs` |

The rest are moving to it one by one, and this list grows as they do.

---

### 🌬️ zephyr-installer

[![PyPI](https://img.shields.io/pypi/v/zephyr-installer)](https://pypi.org/project/zephyr-installer/)

The same one command for Zephyr and nRF Connect SDK. [zephyr-installer](https://github.com/nimaltd/zephyr-installer) makes the library a Zephyr module of your application, adds it to your `CMakeLists.txt` and switches it on in `prj.conf`, with its settings in Kconfig. Every installer here reads the same `installer.yml`, so one library can go into an STM32 project, a Zephyr application, an ESP-IDF project, an Arduino sketch or a PlatformIO project alike, and `--uninstall` takes it out again.

```bash
pip install zephyr-installer
zephyr-installer nimaltd/zephyr-installer-example
```

That one is [zephyr-installer-example](https://github.com/nimaltd/zephyr-installer-example), a small library made for trying the installer on: it builds in any Zephyr application, `native_sim` included, with its settings in Kconfig.

---

### 📶 esp32-installer

[![PyPI](https://img.shields.io/pypi/v/esp32-installer)](https://pypi.org/project/esp32-installer/)

The same one command for ESP-IDF, on any ESP32 chip. [esp32-installer](https://github.com/nimaltd/esp32-installer) makes the library a component in your project's `components` folder, with its own `CMakeLists.txt`, its settings in `idf.py menuconfig`, and the symbols it needs in `sdkconfig.defaults`. Then `idf.py build` picks it up like any other component.

```bash
pip install esp32-installer
esp32-installer nimaltd/esp32-installer-example
```

That one is [esp32-installer-example](https://github.com/nimaltd/esp32-installer-example), a small library made for trying the installer on: a period that never blocks, with its settings in menuconfig.

---

### ♾️ arduino-installer

[![PyPI](https://img.shields.io/pypi/v/arduino-installer)](https://pypi.org/project/arduino-installer/)

The same one command for the Arduino IDE and arduino-cli. [arduino-installer](https://github.com/nimaltd/arduino-installer) puts the library where you choose: in the libraries folder of your sketchbook, for every sketch, with the `library.properties` Arduino knows it by, or in one sketch's `src` folder, for that sketch alone.

```bash
pip install arduino-installer
arduino-installer nimaltd/arduino-installer-example
```

That one is [arduino-installer-example](https://github.com/nimaltd/arduino-installer-example), a small library made for trying the installer on: it builds for any board and prints on Serial.

---

### 🧩 pio-installer

[![PyPI](https://img.shields.io/pypi/v/pio-installer)](https://pypi.org/project/pio-installer/)

The same one command for PlatformIO, with any framework. [pio-installer](https://github.com/nimaltd/pio-installer) puts the library into your project's `lib` folder with the `library.json` PlatformIO builds it by, and the defines it needs into `platformio.ini`, for every environment. Arduino, ESP-IDF, STM32Cube, or no framework at all on the native platform.

```bash
pip install pio-installer
pio-installer nimaltd/pio-installer-example
```

That one is [pio-installer-example](https://github.com/nimaltd/pio-installer-example), a small library made for trying the installer on: it builds with every framework, and runs on your computer on the native platform, with no board at all.

---

### 🎁 Open source, for real

Every library I publish is free and open source. It's my way of giving something back to the embedded community that taught me so much over the years.

If a library saves you time, a ⭐ on the repo or a small [donation on Ko-fi](https://ko-fi.com/nimaltd) means a lot to me. It's a small thing for you, but it genuinely keeps me motivated to keep writing, documenting and maintaining these libraries.

---

### 🏆 Background

- Over 20 years across embedded programming, electronics design and hardware testing
- 🥉 Third place, National Skills Competition of Electronic Engineering, Iran, 2003
- B.Sc. in Electronic Engineering, Chamran University, Rasht

---

### 🌐 Let's connect

[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://www.github.com/NimaLTD)
[![YouTube](https://img.shields.io/badge/YouTube-Subscribe-red?style=for-the-badge&logo=youtube)](https://www.youtube.com/@NimaLTD)
[![Instagram](https://img.shields.io/badge/Instagram-Follow-purple?style=for-the-badge&logo=instagram)](https://www.instagram.com/github.NimaLTD)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/nimaltd)
[![Email](https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail)](mailto:nima.askari@gmail.com)
[![Ko-fi](https://img.shields.io/badge/Ko--fi-Support-orange?style=for-the-badge&logo=ko-fi)](https://ko-fi.com/nimaltd)

---

### 🙏 Thanks

Thanks for stopping by. If any of my work is useful to you, a star on the repo or a small donation helps more than you'd think, and I appreciate every bit of it. ⚙️
