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

| Number | [Arduino Nano](ca://s?q=Arduino_Nano) | Main controller for LEDs + sound | £ | [AE](google.com) |
|--------|----------------------------------------|----------------------------------|---|------------------|
| 1 | [WS2812B LED Strip](ca://s?q=WS2812B_LED_strip) | Blade lighting | £ | [AE](google.com) |
| 1 | [DFPlayer Mini](ca://s?q=DFPlayer_Mini_lightsaber_sound) | Plays MP3 sound effects | £ | [AE](google.com) |
| 1 | [PAM8302 Amp](ca://s?q=PAM8302_audio_amplifier) | Boosts audio to speaker | £ | [AE](google.com) |
| 1 | [8Ω 2W Speaker](ca://s?q=8_ohm_2W_speaker) | Outputs sound | £ | [AE](google.com) |
| 1 | [Micro‑SD Card](ca://s?q=Micro_SD_card) | Stores MP3 sound files | £ | [AE](google.com) |
| 1 | [MT3608 Boost Converter](ca://s?q=MT3608_boost_converter) | Boosts AA battery voltage to 5V | £ | [AE](google.com) |
| 1 | [3× AA Battery Holder](ca://s?q=AA_battery_holder) | Powers the saber | £ | [AE](google.com) |
| 2 | [Momentary Buttons](ca://s?q=Momentary_push_buttons) | Main power + extra sound | £ | [AE](google.com) |
| 1 | [Clear PVC Blade Tube](ca://s?q=Clear_PVC_blade_tube) | Saber blade | £ | [AE](google.com) |
| 1 | [Baking Paper](ca://s?q=Baking_paper_diffuser) | Blade diffusion | £ | [AE](google.com) |
| 1 | [Reflective Tip](ca://s?q=Reflective_blade_tip) | Brightens blade end | £ | [AE](google.com) |
| 1 | [3D‑Printed Hilt](ca://s?q=3D_printed_lightsaber_hilt) | Holds all electronics | £ | [AE](google.com) |
| — | [Wires + Heat‑shrink](ca://s?q=Electronics_wires_heatshrink) | General wiring | £ | [AE](google.com) |


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


