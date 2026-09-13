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

## Parts List

### Electronics
- Arduino Nano  
- WS2812B LED strip  
- MT3608 boost converter (set to 5V)  
- 3× AA battery holder  
- Momentary push buttons (x2)  
- Wiring + heat‑shrink  

### Sound System
- DFPlayer Mini  
- PAM8302 amplifier  
- 8Ω 2W speaker  
- Micro‑SD card (for sound files)

### Blade + Hilt
- Clear PVC tube  
- Baking paper (diffusion)  
- Reflective blade tip (foil or aluminium tape)  
- 3D‑printed hilt  
- Blade holder

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


