<!-- omit in toc -->
# Awesome ESP Rust

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

> A curated list of resouces for development in the Rust programming language for ESP32, ESP32-C2/C3/C6, ESP32-H2, and ESP32-S2/S3.

<!-- omit in toc -->
## Table of Contents

- [Community](#community)
- [Books, Blogs, and Training Materials](#books-blogs-and-training-materials)
- [Video Courses and Talks](#video-courses-and-talks)
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
- [EN] [Embedded Rust (std) on Espressif](https://esp-rs.github.io/std-training/) - Training for Rust using `std` approach development on ESP32-C3 by [Ferrous Systems](https://ferrous-systems.com/training/).
- [EN] [Embedded Rust (no_std) on Espressif](https://esp-rs.github.io/no_std-training/) - Training for Rust using `no_std` approach development on ESP32-C3.
- [EN] [Espressif Developer Portal - tag: Rust](https://developer.espressif.com/tags/rust/) - Articles about Rust for ESP32.
- [EN] [Scott Mabin - Rust on Espressif chips](https://mabez.dev/blog/posts/) - Quarterly updates about Rust on Espressif chips.
- [EN] Making a Dino Light with the ESP32 and WS2812
  - [Making a Dino Light with the ESP32 and WS2812](https://nereux.blog/posts/esp32-ws2812-dino-light/)
  - [Making a Dino Light with the ESP32 and WS2812 Pt. 2](https://nereux.blog/posts/esp32-ws2812-dino-light-2/)
- [EN] [ESP32 with Embedded Rust at the HAL](https://blog.theembeddedrustacean.com/series/esp32c3-embedded-rust-hal/) - Blog series about learning Rust at the HAL level with the ESP32-C3.
- [EN] [A getting started guide to ESP32 no-std Rust development](https://nereux.blog/posts/getting-started-esp32-nostd/)
- [EN] [impl Rust on ESP32](https://esp32.implrust.com/) - The book explores and explains various exciting projects using an ESP32.
- [JP] 倒立振子ロボットを現代制御で動かしたい (I want to run an inverted pendulum robot with modern control)
  - [(1) モデル化](https://zenn.dev/tana_ash/articles/balance-robot-modern-1) (Modelling)
  - [(2) 直立制御](https://zenn.dev/tana_ash/articles/balance-robot-modern-2) (Upright Control)
  - [(3) 遠隔操縦](https://zenn.dev/tana_ash/articles/balance-robot-modern-3) (Remote Control)
- [JP] ESP32 で std な Rust 開発入門
  - [その 1 環境構築](https://lang-ship.com/blog/work/esp32-std-rust-1/) (Part 1: Building the environment)
  - [その 2 L チカ](https://lang-ship.com/blog/work/esp32-std-rust-2/) (Part 2: Blink an LED)
- [EN] [Programming ESP32 with Rust: OTA firmware update](https://quan.hoabinh.vn/post/2024/3/programming-esp32-with-rust-ota-firmware-update)
- [VI] [Lập trình ESP32 với Rust: cập nhật firmware OTA](https://quan.hoabinh.vn/post/2024/03/lap-trinh-esp32-voi-rust-cap-nhat-firmware-ota)
- [EN] [Securely sending DHT22 sensor data from an ESP32 board to PostgreSQL](https://c410-f3r.github.io/thoughts/securely-sending-dht22-sensor-data-from-an-esp32-board-to-postgresql/)
- [EN] [Freenove ESP32 Tutorials in Rust](https://makuo12.github.io/Freenove-esp32-rust/) - Transforms traditional C and MicroPython-based Freenove lessons into idiomatic Rust code.
## Video Courses and Talks

- [EN] [Rust on ESP32-C3](https://www.youtube.com/playlist?list=PLkch9g9DEE0Lkm1LqcD7pZNDmXEczOo-a)
- [EN] [Andrei Litvin / @embedded-rust](https://www.youtube.com/@embedded-rust/videos)
- [EN] [Rust embedded at Espressif @ Copenhagen Rust Community](https://www.youtube.com/watch?v=gdmUhzJfgzk)
- [EN] [Embedded Rust on ESP32 - Juraj Michálek - Rust Linz November 2022](https://www.youtube.com/watch?v=0PPPdqoDBQs)
- [EN] [Rust on Espressif chips - Scott Mabin - DevCon22](https://www.youtube.com/watch?v=qeEmJ_-6fPg)
- [EN] [Rust Bare-metal and Async - Scott Mabin, Juraj Sadel - DevCon23](https://www.youtube.com/watch?v=QPp4WEjx5jU)
- [EN] [Rust on ESP32 - Video series live coding esp32 examples in Rust](https://www.youtube.com/playlist?list=PL0U7YUX2VnBFbwTi96wUB1nZzPVN3HzgS)
## Tools

- [espup](https://github.com/esp-rs/espup) - Tool for installing and maintaining the required toolchains for developing applications in Rust for Espressif SoC's.
- [espflash](https://github.com/esp-rs/espflash) - Serial flasher utility for Espressif SoCs and modules based on [esptool](https://github.com/espressif/esptool).
- [esp-web-flash-server](https://github.com/bjoernQ/esp-web-flash-server) - WebSocket server for flashing from Visual Studio Code Remote Containers using a web browser.
- [wokwi-server](https://github.com/MabezDev/wokwi-server) - WebSocket server for running simulations in [Wokwi](https://wokwi.com/) from Visual Studio Code Remote Containers using a web browser.
- [Wokwi Simulator](https://wokwi.com/rust) - Web browser simulator that supports Rust language on ESP32 chips.

## Templates

- [esp-idf-template](https://github.com/esp-rs/esp-idf-template) - A [cargo-generate](https://cargo-generate.github.io/cargo-generate/) template for projects using the Rust `std` library (via [ESP-IDF](https://github.com/espressif/esp-idf)).
- [esp-generate](https://github.com/esp-rs/esp-generate) - Template generation tool to create `no_std` applications targeting Espressif's chips.

## Open Hardware

- [esp-rust-board](https://github.com/esp-rs/esp-rust-board) - A development board based on the ESP32-C3 and designed in [KiCad EDA](https://www.kicad.org/) which is compatible with the [Adafruit Feather](https://learn.adafruit.com/adafruit-feather/feather-specification) specification.

## Projects

### `std`

- [anemometer](https://github.com/taunusflieger/anemometer) - Rust based anemometer incl. OTA and GPS based calibration process.
- [bluedroid](https://github.com/pulse-loop/bluedroid) - Safe wrapper for the Bluedroid Bluetooth stack.
- [Dark Sky Meter](https://gitlab.com/scrobotics/optical-makerspace/dark-sky-meter-fw) - Open Hardware low-cost night sky sensor that measures light levels as well as several ambient parameters.
- [dephy-esp32c3-rust-boilerplate](https://github.com/dephy-io/dephy-esp32c3-rust-boilerplate) - A `std` ESP32-C3 application boilerplate on production with `tokio` for `async` support and examples for IO, Wi-Fi provisioning, eFuse, GPIO, I2C, HTTP, BLE advertising, etc.
- [esp-clock](https://github.com/playfulFence/esp-clock) - Clock with environment stats. [Wokwi project](https://wokwi.com/projects/357451677483992065)
- [esp32-idf-nmea-example](https://github.com/georgik/esp32-idf-nmea-example) - Example of integration ESP-IDF application with Rust code as component.
- [esp32-s3-rust-axum-example](https://github.com/aedm/esp32-s3-rust-axum-example) - Example of running Tokio + Axum web server on the ESP32-S3.
- [esp32c3-rust-std-temperature-logger](https://github.com/bjoernQ/esp32c3-rust-std-temperature-logger) - MQTT temperature logger running on ESP32-C3.
- [esp32cam-rs](https://github.com/Kezii/esp32cam_rs) - Examples of Rust on ESP32-CAM, including a fully-featured Telegram bot capable of taking pictures.
- [gateway-rs](https://github.com/OpenIoTHub/gateway-rs) - A fast reverse proxy to help you expose a local server behind a NAT or firewall to the internet(like [frp](https://github.com/fatedier/frp) but running on ESP32).
- [mch2022-rust-app](https://github.com/p2mate/mch2022-rust-app) - Example that shows a nice rust screensaver in MCH2022 badge.
- [M5Stack-Cardputer](https://github.com/Kezii/Rust-M5Stack-Cardputer) - Rust support for the Cardputer, including an interactive 3d graphics demo
- [OFMon](https://github.com/arashsm79/OFMon) - Offline-first smart energy monitor using littlefs, Rust, ESP32, and Thingsboard. [See details](https://moslehian.com/posts/2022/3-ofmon/).
- [OxidESPark](https://gitlab.com/cyril-marpaud/oxide-spark) - Rust library for the Rust ESP Board that uses the ESP-IDF framework and provides tools to easily build applications that interact with the physical world.
- [rust-esp32-std-demo](https://github.com/ivmarkov/rust-esp32-std-demo) - A demo `std` binary crate for the ESP32[XX] and [ESP-IDF](https://github.com/espressif/esp-idf), which connects to WiFi, Ethernet, drives a small HTTP server and draws on a LED screen.
- [rust4mch](https://github.com/jhaand/rust4mch) - Example to run Rust code on the MCH2022 badge.
- [rustzx-esp32](https://github.com/georgik/rustzx-esp32) - ZX Spectrum emulator based on RustZX project.
- [self-balancing robot](https://github.com/tana/atom-motion-balance) - Self-balancing robot using Atom Matrix and Atom Motion. [See details](https://zenn-dev.translate.goog/tana_ash/articles/5a458538cd9204?_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en-US&_x_tr_pto=wapp).
- [twatch-idf-rs](https://github.com/pyaillet/twatch-idf-rs) - Experimental firmware for the Lilygo T-Watch
- [wrover-experimental](https://github.com/JurajSadel/wrover-experimental) - Display line directions and departure times of public transport vehicles in Brno, CZ.
- [esp-clock-rs](https://github.com/zhangzqs/esp-clock-rs) - A weather clock project designed based on the Slint UI framework. This is a attempt for the low-coupling cross-platform project based on the message communication mechanism, which supports running on ESP32-C3, WebBrowser(WASM), Desktop, and Android.

### `no_std`

- [esp32c3-devkit-rust - Embassy, BLE, Sensors example](https://github.com/jamessizeland/esp32c3-devkit-demo) - Medium complexity project demo interfacing with the peripherals available on this board, which include RGB LED, i2c IMU, Temperature & Humidity and BLE using TrouBLE and Embassy.
- [esp32 wifi tank](https://jamesmcm.github.io/blog/esp32-wifi-tank/) - Building a Wifi-controlled car with Rust and ESP32
- [Beginner Rust ESP32 development - Snake](https://jamesmcm.github.io/blog/beginner-rust-esp32-lcdsnake/) - Snake game to run on an ESP32 development board with a connected OLED display and controlled with a joystick.
- [esp32-rust-nostd-temperature-logger](https://github.com/bjoernQ/esp32-rust-nostd-temperature-logger) - MQTT temperature logger running on ESP32.
- [esp32-conways-game-of-life-rs](https://github.com/georgik/esp32-conways-game-of-life-rs) - Conway's Game of Life in Bare metal Rust for different ESP32 based boards.
- [esp32-spooky-maze-game](https://github.com/georgik/esp32-spooky-maze-game) - Bare metal Rust implementation of game for different ESP32 based boards using Bevy ECS no_std.
- [esp32-rex](https://github.com/ImplFerris/esp32-rex) - Dinosaur Game written in Rust for the ESP32 with an OLED display, using the Embassy framework.
- [ps2keyboard-esp32c3](https://github.com/bjoernQ/ps2keyboard-esp32c3) - PS/2 keyboard implementation for ESP32-C3.
- [esp32c3-ota-experiment](https://github.com/bjoernQ/esp32c3-ota-experiment) - ESP32-C3 Bare Metal OTA Experiment.
- [SlimeVR-Rust/firmware](https://github.com/SlimeVR/SlimeVR-Rust/tree/main/firmware) - Async & no_std rust firmware for SlimeVR Full Body Tracking.
- [esp32s3-box-examples](https://github.com/sambenko/esp32s3-box-examples) - Various graphic examples for ESP32-S3 Box.
- [nostd-wifi-lamp](https://github.com/Nereuxofficial/nostd-wifi-lamp) - A Wi-Fi Lamp built with an ESP32 and Neopixel Lights controllable via Wi-Fi
- [plantineers-edge](https://github.com/plantineers/edge) - Firmware for edge devices for an Open Source Plant Monitoring solution using esp-now
- [esp32c3-no-std-async-mqtt-demo](https://github.com/JurajSadel/esp32c3-no-std-async-mqtt-demo) - ESP32-C3 application that measures temperature (using BMP180) and sends the results with MQTT via WiFi - everything is done asynchronously. Also available for [ESP32](https://github.com/JurajSadel/esp32-no-std-async-mqtt-demo) and [ESP32-S3](https://github.com/JurajSadel/esp32s3-no-std-async-mqtt-demo)
- [esp32-rust-lilygo-t5-epaper](https://github.com/georgik/esp32-rust-lilygo-t5-epaper) - ESP32 LilyGo T5 ePaper with WiFi
- [esp32-buddy-rs](https://github.com/georgik/esp32-buddy-rs) - Bare metal Rust examples for ESP-Buddy board
- [bradipograph](https://github.com/jneem/bradipograph/) - A sloth-like drawing robot.
- [esp-examples](https://github.com/danclive/esp-examples) - Some examples of esp-hal.
- [touch-n-drink](https://github.com/zargony/touch-n-drink) - Cashless payment device for cold drinks at a German aeroclub
- [tetris](https://github.com/Hahihula/no_std_tetris) - simple tetris implementation on esp32-c3 and neopixels led strip
- [esp-hub75](https://github.com/liebman/esp-hub75) - driver for Hub75 Matrix RGB LED Displays supporting ESP32, ESP32-S3, and ESP32-C6
- [esp32-mipidsi-clock](https://github.com/mgrenonville/esp32-mipidsi-clock) - A Round LCD clock with slint UI + embassy, NTP time sync via WIFI, and SVG rendering on ESP32-C6
- [esp-rust-spi-lcd-demo](https://github.com/KaidRommel/esp-rust-spi-lcd-demo) - A demonstration project for the ESP32-S3, showcasing a bouncing text animation on an SPI LCD.


## License

This list is licensed under

- CC0 1.0 Universal License ([LICENSE](LICENSE) or https://creativecommons.org/publicdomain/zero/1.0/legalcode)
