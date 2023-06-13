<!-- omit in toc -->
# Awesome ESP Rust

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

> A curated list of resouces for development in the Rust programming language for ESP32, ESP32-C2/C3/C6, and ESP32-S2/S3.

<!-- omit in toc -->
## Table of Contents

- [Community](#community)
- [Books, Blogs, and Training Materials](#books-blogs-and-training-materials)
- [Video Courses](#video-courses)
- [Tools](#tools)
- [Templates](#templates)
- [Open Hardware](#open-hardware)
- [Projects](#projects)
  - [`std`](#std)
  - [`no_std`](#no_std)
- [License](#license)

## Community

You can usually find community members (including some employees of Espressif) in the [`#esp-rs:matrix.org` Matrix room](https://matrix.to/#/#esp-rs:matrix.org).

## Books, Blogs, and Training Materials

- [EN] [The Rust on ESP Book](https://esp-rs.github.io/book/introduction.html) - The goal of this book is to provide a comprehensive guide on using the Rust programming language with Espressif SoCs and modules.
- [EN] [Embedded Rust on Espressif](https://esp-rs.github.io/std-training/) - Training for Rust development on ESP32-C3 by [Ferrous Systems](https://ferrous-systems.com/training/).
- [EN] [Scott Mabin - Rust on Espressif chips](https://mabez.dev/blog/posts/) - Quarterly updates about Rust on Espressif chips.
- [EN] [Bare-Metal Rust on ESP32: A brief overview](https://beta7.io/posts/bare-metal-rust-on-esp32/) - Overview of the `no_std` ecosystem on ESP32 chips.
- [EN] Making a Dino Light with the ESP32 and WS2812
  - [Making a Dino Light with the ESP32 and WS2812](https://nereux.blog/posts/esp32-ws2812-dino-light/)
  - [Making a Dino Light with the ESP32 and WS2812 Pt. 2](https://nereux.blog/posts/esp32-ws2812-dino-light-2/)
- [EN] [ESP32 with Embedded Rust at the HAL](https://apollolabsblog.hashnode.dev/series/esp32c3-embedded-rust-hal) - Blog series about learning Rust at the HAL level with the ESP32-C3.
- [JP] 倒立振子ロボットを現代制御で動かしたい (I want to run an inverted pendulum robot with modern control)
  - [(1) モデル化](https://zenn.dev/tana_ash/articles/balance-robot-modern-1) (Modelling)
  - [(2) 直立制御](https://zenn.dev/tana_ash/articles/balance-robot-modern-2) (Upright Control)
  - [(3) 遠隔操縦](https://zenn.dev/tana_ash/articles/balance-robot-modern-3) (Remote Control)
- [JP] ESP32 で std な Rust 開発入門
  - [その 1 環境構築](https://lang-ship.com/blog/work/esp32-std-rust-1/) (Part 1: Building the environment)
  - [その 2 L チカ](https://lang-ship.com/blog/work/esp32-std-rust-2/) (Part 2: Blink an LED)

## Video Courses

- [EN] [Rust on ESP32-C3](https://www.youtube.com/playlist?list=PLkch9g9DEE0Lkm1LqcD7pZNDmXEczOo-a)
- [EN] [Andrei Litvin / @embedded-rust](https://www.youtube.com/@embedded-rust/videos)

## Tools

- [espup](https://github.com/esp-rs/espup) - Tool for installing and maintaining the required toolchains for developing applications in Rust for Espressif SoC's.
- [espflash](https://github.com/esp-rs/espflash) - Serial flasher utility for Espressif SoCs and modules based on [esptool](https://github.com/espressif/esptool).
- [esp-web-flash-server](https://github.com/bjoernQ/esp-web-flash-server) - WebSocket server for flashing from Visual Studio Code Remote Containers using a web browser.
- [wokwi-server](https://github.com/MabezDev/wokwi-server) - WebSocket server for running simulations in [Wokwi](https://wokwi.com/) from Visual Studio Code Remote Containers using a web browser.
- [Wokwi Simulator](https://wokwi.com/rust) - Web browser simulator that supports Rust language on ESP32 chips.

## Templates

- [esp-idf-template](https://github.com/esp-rs/esp-idf-template) - A [cargo-generate](https://cargo-generate.github.io/cargo-generate/) template for projects using the Rust `std` library (via [ESP-IDF](https://github.com/espressif/esp-idf)).
- [esp-template](https://github.com/esp-rs/esp-template) - A [cargo-generate](https://cargo-generate.github.io/cargo-generate/) template for bare metal projects (ie. `no_std`).

## Open Hardware

- [esp-rust-board](https://github.com/esp-rs/esp-rust-board) - A development board based on the ESP32-C3 and designed in [KiCad EDA](https://www.kicad.org/) which is compatible with the [Adafruit Feather](https://learn.adafruit.com/adafruit-feather/feather-specification) specification.

## Projects

### `std`

- [anemometer](https://github.com/taunusflieger/anemometer) - Rust based anemometer incl. OTA and GPS based calibration process.
- [bluedroid](https://github.com/pulse-loop/bluedroid) - Safe wrapper for the Bluedroid Bluetooth stack.
- [esp-clock](https://github.com/playfulFence/esp-clock) - Clock with environment stats. [Wokwi project](https://wokwi.com/projects/357451677483992065)
- [esp32c3-rust-std-temperature-logger](https://github.com/bjoernQ/esp32c3-rust-std-temperature-logger) - MQTT temperature logger running on ESP32-C3.
- [gateway-rs](https://github.com/OpenIoTHub/gateway-rs) - A fast reverse proxy to help you expose a local server behind a NAT or firewall to the internet(like [frp](https://github.com/fatedier/frp) but running on ESP32).
- [mch2022-rust-app](https://github.com/p2mate/mch2022-rust-app) - Example that shows a nice rust screensaver in MCH2022 badge.
- [OFMon](https://github.com/arashsm79/OFMon) - Offline-first smart energy monitor using littlefs, Rust, ESP32, and Thingsboard. [See details](https://moslehian.com/posts/2022/3-ofmon/).
- [rust-esp32-std-demo](https://github.com/ivmarkov/rust-esp32-std-demo) - A demo `std` binary crate for the ESP32[XX] and [ESP-IDF](https://github.com/espressif/esp-idf), which connects to WiFi, Ethernet, drives a small HTTP server and draws on a LED screen.
- [rust4mch](https://github.com/jhaand/rust4mch) - Example to run Rust code on the MCH2022 badge.
- [rustzx-esp32](https://github.com/georgik/rustzx-esp32) - ZX Spectrum emulator based on RustZX project.
- [self-balancing robot](https://github.com/tana/atom-motion-balance) - Self-balancing robot using Atom Matrix and Atom Motion. [See details](https://zenn-dev.translate.goog/tana_ash/articles/5a458538cd9204?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en-US&_x_tr_pto=wapp).
- [twatch-idf-rs](https://github.com/pyaillet/twatch-idf-rs) - Experimental firmware for the Lilygo T-Watch
- [wrover-experimental](https://github.com/JurajSadel/wrover-experimental) - Display line directions and departure times of public transport vehicles in Brno, CZ.

### `no_std`

- [esp32-rust-nostd-temperature-logger](https://github.com/bjoernQ/esp32-rust-nostd-temperature-logger) - MQTT temperature logger running on ESP32.
- [esp32-spooky-maze-game](https://github.com/georgik/esp32-spooky-maze-game) - Bare metal Rust implementation of simple game for ESP32.
- [ps2keyboard-esp32c3](https://github.com/bjoernQ/ps2keyboard-esp32c3) - PS/2 keyboard implementation for ESP32-C3.
- [esp32c3-ota-experiment](https://github.com/bjoernQ/esp32c3-ota-experiment) - ESP32-C3 Bare Metal OTA Experiment.
- [SlimeVR-Rust/firmware](https://github.com/SlimeVR/SlimeVR-Rust/tree/main/firmware) - Async & no_std rust firmware for SlimeVR Full Body Tracking.
- [esp32s3-box-examples](https://github.com/sambenko/esp32s3-box-examples) - Various graphic examples for ESP32-S3 Box.
- [nostd-wifi-lamp](https://github.com/Nereuxofficial/nostd-wifi-lamp) - A Wi-Fi Lamp built with an ESP32 and Neopixel Lights controllable via Wi-Fi
- [plantineers-edge](https://github.com/plantineers/edge) - Firmware for edge devices for an Open Source Plant Monitoring solution using esp-now

## License

This list is licensed under

- CC0 1.0 Universal License ([LICENSE](LICENSE) or https://creativecommons.org/publicdomain/zero/1.0/legalcode)
