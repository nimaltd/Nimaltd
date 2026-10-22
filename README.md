# 👋 Hi, I'm Nima Askari

I'm an electronics engineer and embedded systems developer. For more than 20 years I've been writing C for STM32 microcontrollers, and most of that time has gone into one goal: making libraries that are actually easy to use.

I got tired of fighting messy drivers and overcomplicated code, so I started writing my own, cleaning them up, and sharing them with anyone who needs them.

---

### 💡 What I focus on

Lightweight, non-blocking, easy to drop in C libraries for STM32 (HAL and LL), covering storage, communication, sensors and general drivers. The idea is always the same: add the library to your project and have it working in minutes, not days.

That is what lib-installer below is for: one command puts a library into an STM32, Zephyr, ESP-IDF, Arduino or PlatformIO project. It works with anyone's library, not only mine, once it has an `installer.yml`. It takes a library and what it needs from GitHub, one release of it with `owner/name@v1.2.0`, or a zip when there is no internet, and asks before it runs anything a library brings, such as a script that makes a signing key.

---

### 🧰 lib-installer

[![PyPI](https://img.shields.io/pypi/v/lib-installer)](https://pypi.org/project/lib-installer/)

Installing one of my libraries takes one command, on every platform. [lib-installer](https://github.com/nimaltd/lib-installer) copies the files into your project and adds the library to its build, backing up every project file first. Any library it needs comes with it, an update keeps your settings, and `--uninstall` takes it out again. The library's `installer.yml` says which platform it is for, so the command is the same everywhere.

```bash
pip install lib-installer
lib-installer nimaltd/ee24
```

| Platform | What it does | Try it with |
|---|---|---|
| STM32 | Adds the library to your CMake, STM32CubeIDE, Keil, IAR or Makefile project | `lib-installer nimaltd/lib-installer-example-stm32` |
| Zephyr and nRF Connect SDK | Makes it a Zephyr module, adds it to `CMakeLists.txt` and switches it on in `prj.conf`, with its settings in Kconfig | `lib-installer nimaltd/lib-installer-example-zephyr` |
| ESP-IDF | Makes it a component, with its settings in `idf.py menuconfig` and the symbols it needs in `sdkconfig.defaults` | `lib-installer nimaltd/lib-installer-example-esp32` |
| Arduino | Puts it in your sketchbook's libraries folder, or one sketch's `src` folder, with the `library.properties` Arduino needs | `lib-installer nimaltd/lib-installer-example-arduino` |
| PlatformIO | Puts it in `lib` with a `library.json`, and the defines it needs in `platformio.ini`, for every framework | `lib-installer nimaltd/lib-installer-example-pio` |

Each of the last column is a small library made for trying the installer on, a period that never blocks, which builds on its platform with nothing to set up.

Libraries you can install with it:

| Library | Description | Install |
|---|---|---|
| [seq](https://github.com/nimaltd/seq) | Non blocking state sequencer and interrupt task queue for STM32 | `lib-installer nimaltd/seq` |
| [ee24](https://github.com/nimaltd/ee24) | Driver for 24xx I2C EEPROMs, 24C01 to 24C512, on the STM32 HAL | `lib-installer nimaltd/ee24` |
| [spif](https://github.com/nimaltd/spif) | Driver for SPI NOR flash, W25Qxx and compatible, on the STM32 HAL | `lib-installer nimaltd/spif` |
| [osal](https://github.com/nimaltd/osal) | OS abstraction layer for STM32: the same tasks, mutexes, critical sections, delays and heap on bare metal, FreeRTOS and ThreadX | `lib-installer nimaltd/osal` |
| [littlefs](https://github.com/nimaltd/littlefs) | LittleFS by the littlefs project, ready for lib-installer | `lib-installer nimaltd/littlefs` |

The rest are moving to it one by one, and this list grows as they do. stm32-installer, zephyr-installer, esp32-installer, arduino-installer and pio-installer were five installers until 3.0.0, and are lib-installer now: a project one of them installed into moves over by itself.

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
