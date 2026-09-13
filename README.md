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
| 1 | Arduino Nano | Main microcontroller for LEDs + sound | £ | [link](google.com) |
| 1 | WS2812B LED Strip | Blade lighting | £ | [link](google.com) |
| 1 | DFPlayer Mini | Plays MP3 sound effects | £ | [link](google.com) |
| 1 | PAM8302 Amplifier | Boosts audio to speaker | **OWN** | N/A |
| 1 | 8Ω 2W Speaker | Outputs sound | £ | [link](google.com) |
| 1 | Micro‑SD Card | Stores MP3 sound files | **OWN** | N/A |
| 1 | MT3608 Boost Converter | Boosts AA battery voltage to 5V | **OWN** | N/A |
| 1 | 4× AA Battery Holder | Powers the saber | £ | [AE](https://www.aliexpress.com/item/1005009290619005.html?spm=a2g0o.productlist.main.6.462a7bbdifoQlS&algo_pvid=5e401952-e62b-4a6a-876a-1445e0d1deb9&algo_exp_id=5e401952-e62b-4a6a-876a-1445e0d1deb9-5&pdp_ext_f=%7B%22order%22%3A%2226%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21GBP%211.38%211.33%21%21%2112.17%2111.73%21%4021613be817893155341732043e0e32%2112000048630566995%21sea%21GB%217850874718%21X%211%210%21n_tag%3A-29919%3Bd%3Ac7b67d0a%3Bm03_new_user%3A-29895&curPageLogUid=0e5n3crJ5sqd&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005009290619005%7C_p_origin_prod%3A) |
| 2 | Momentary Buttons | Main power + extra sound | £ | [link](google.com) |
| 1 | Clear PVC Blade Tube | Saber blade | £ | [link](google.com) |
| 1 | Baking Paper | Blade diffusion | £ | [link](google.com) |
| 1 | Reflective Blade Tip | Brightens blade end | £ | [link](google.com) |
| 1 | 3D‑Printed Hilt | Holds all electronics | £ | N/A |
| — | Wires + Heat‑shrink | General wiring | £ | [link](google.com) |


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


