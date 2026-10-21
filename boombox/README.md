# Lilka Boombox

A music player firmware for the **Lilka v2** handheld console (ESP32-S3):
SD card music with a live spectrum, plus internet radio
https://github.com/vaddieg/lilka-boombox

## Features

- **SD music** — browse `/music` (subfolders allowed), play/pause/prev/next,
  volume, and **shuffle** (press again to restore the original order).
- **Internet radio** — user station list from the SD card, or a built-in
  fallback list. Stream titles shown when the server sends them (ICY).
- **15-band live spectrum** and a stepped color volume meter.

## Supported formats

`mp3`, `m4a`, `aac`, `wma`, `flac`, `wav`, `ogg`, `mid`

## SD card layout

```
/music/            songs (any subfolder structure)
/webradio/         station files, one per station:
   <Name>.url      first line = stream URL, filename = station name
```

## Installation

Download the BIN file and copy it to the Lilka's SD card. Launch from Keira OS.