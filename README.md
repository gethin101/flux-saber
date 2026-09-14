# Flux Saber

A DIY lightsaber project built using an Arduino Nano, WS2812B LEDs, and a DFPlayer Mini sound module.  
The goal is to create a bright, smooth‑lighting blade with simple, reliable sound effects inside a 3D‑printed hilt.

---

## Vision

Flux Saber aims to be a clean, functional lightsaber with:
- smooth ignition and shutdown lighting
- steady blade glow
- basic sound effects (on, hum, off, extra button sound)
- a compact internal layout powered by AA batteries boosted to 5V

---

# BOM

| Number | Name | Use | Price | Link |
|--------|------|-----|--------|------|
| 1 | Arduino Nano (c) | Main microcontroller for LEDs + sound | £1.80 | [AE](https://www.aliexpress.com/item/1005005128673508.html) |
| 1 | WS2812B LED Strip (60 IP65 1m) | Blade lighting | £3.20 | [AE](https://www.aliexpress.com/item/1005003151401311.html) |
| 1 | DFPlayer Mini | Plays MP3 sound effects | £1.93 | [AE](https://www.aliexpress.com/item/1005010550604358.html) |
| 1 | PAM8302 Amplifier | Boosts audio to speaker | **OWN** | N/A |
| 1 | 8Ω 2W Speaker | Outputs sound | **OWN** | N/A) |
| 1 | Micro‑SD Card | Stores MP3 sound files | **OWN** | N/A |
| 1 | MT3608 Boost Converter | Boosts AA battery voltage to 5V | **OWN** | N/A |
| 1 | 4× AA Battery Holder | Powers the saber | £1.33 | [AE](https://www.aliexpress.com/item/1005009290619005.html) |
| 2 | Tactile buttons | Control special effects | **OWN** | N/A |
| 1 | KCD11 rocker switch | Power kill switch | **OWN** | N/A |
| 1 | Clear PVC Blade Tube | Saber blade | £ | [link](google.com) |
| 1 | Baking Paper | Blade diffusion | **OWN** | N/A |
| 1 | Reflective Blade Tip | Brightens blade end | £ | [link](google.com) |
| 1 | 3D‑Printed Hilt | Holds all electronics | Filament | N/A |
| 1 | Heat‑shrink tubing (164 bag) | Insulates solder joints | £1.22 | [AE](https://www.aliexpress.com/item/1005008064154315.html( |
| - | Dupont jumper wires | General wiring | **OWN** | N/A |




---

## How It Works

### Power
AA batteries feed the MT3608 boost converter, which outputs a stable 5V.  
This powers the Arduino, LEDs, DFPlayer Mini, and amplifier.

### Lighting
The Arduino drives the WS2812B LED strip to create:
- ignition animation  
- steady blade glow  
- shutdown animation

### Sound
The DFPlayer Mini plays MP3 files stored on the micro‑SD card:
- `001.mp3` → ignition  
- `002.mp3` → hum loop  
- `003.mp3` → shutdown  
- `004.mp3` → extra button sound

The PAM8302 amplifier boosts the audio to the speaker.

### Buttons
- Main button toggles the blade and plays on/off sounds  
- Extra button triggers a custom sound

---

## SD Card Structure
001.mp3   # ignition
002.mp3   # hum loop
003.mp3   # shutdown
004.mp3   # extra button sound


---

## Summary

Flux Saber combines WS2812B LEDs, basic sound playback, and a simple power system to create a bright, responsive DIY lightsaber that fits inside a 3D‑printed hilt.


