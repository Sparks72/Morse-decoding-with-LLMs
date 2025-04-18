# Morse decoding with LLM's

📡 **Browser-Based Morse Code Decoder**  
A self-contained, platform-independent Morse code decoder optimised for noisy conditions. Runs entirely in the browser – no install required.

---

### 🌐 [Live Demo Here](https://sparks72.github.io/Morse-decoding-with-LLMs/)

---

## 🔍 Overview

This tool uses Web Audio API and a Goertzel-based tone detector to decode Morse code from microphone input. It dynamically adapts to:
- Variable transmission speeds (12–40 WPM)
- Frequency shifts (500–900 Hz)
- Noise and weak signals (via adaptive SNR-based thresholding)

All visual feedback is live, including:
- Real-time waveform
- Spectrum analyser
- Signal/Noise confidence meter
- Decoding output buffer

---

## 🖼 Interface Preview

> *(Insert screenshot here – e.g. drag a `.png` of your interface into the repo)*

---

## 🚀 Features

✅ Adaptive Morse decoding  
✅ Auto-tone and speed tracking  
✅ SNR and confidence estimation  
✅ No spurious characters in noisy conditions  
✅ Works offline after first load  
✅ Fully self-contained (HTML + JS)  
✅ Cross-platform: Windows, Linux, macOS, Android, iOS

---

## 🛠 Usage

1. **Open** the decoder: [sparks72.github.io/Morse-decoding-with-LLMs](https://sparks72.github.io/Morse-decoding-with-LLMs/)
2. **Allow microphone** access
3. Click **Start Decoding**
4. Adjust frequency and speed sliders if needed

---

## 📁 Files in this Repo

| File         | Description                             |
|--------------|-----------------------------------------|
| `index.html` | The full app – open this in any browser |
| `README.md`  | This file                              |
| `.gitignore` | (Optional) ignores temp/dev files       |

---

## 🧪 Try It On-Air

Try decoding on:
- 7030 kHz (CW QRP calling freq)
- W1AW CW practice transmissions
- Your own rig with sidetone to mic

Works even with very weak signals!

---

## 🏷 Tags

`morse-code` `ham-radio` `decoder` `javascript` `browser` `LLM` `cw` `web-audio` `goertzel` `qrz` `portable` `no-install`

---

## ⚖️ License

This project is provided freely for educational and amateur radio use.  
Attribution is appreciated – DJ0CU / G4ADF
