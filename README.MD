# About

This is my collection of popular MCU applications ported to the ESP32-based Lilka console: https://lilka.dev.

KeiraOS allows running precompiled ESP32-S3 firmwares from the SD card as if they were regular apps, turning the console into a multi-purpose LoRa/SDR device. Everything I add to this collection is tested with Lilka v2 and extensions listed in the **hardware**.

# Installation

Download a precompiled `.bin` file from the corresponding app directory and copy it to the Lilka SD card. Use "raw" download option on the GitHub to prevent file corruption. Alternatively, compile your own copy of firmwares (see instructions below).

# Hardware

The Lilka console is compatible with a variety of radios and sensors, but you may need to do some soldering to connect them. See the **hardware** directory for details.

# Compilation

The Lilka team is working on upstreaming platform support for popular MCU applications. Until that is available, you can checkout the sources from their official GitHub repositories and manually add the Lilka platform definition files.

