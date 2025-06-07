# Professional Morse Code Decoder with QRZ Integration

![Morse Code Decoder](https://img.shields.io/badge/Morse%20Code-Decoder-blue)
![QRZ Integration](https://img.shields.io/badge/QRZ-Integration-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

A professional-grade web application for decoding Morse code from audio input with adaptive speed, frequency tuning, and automatic ham radio callsign detection with QRZ.com integration.

## 📊 Demo

![screenshot][https://github.com/Sparks72/Morse-decoding-with-LLMs/QRZ-Intergration/screenshot1.png)
![screenshot][https://github.com/Sparks72/Morse-decoding-with-LLMs/QRZ-Intergration/screenshot2.png)
## ✨ Features

### 🎯 Core Functionality
- **Real-time Morse code decoding** from microphone input
- **Adaptive speed detection** (12-40 WPM)
- **Auto-frequency tuning** (500-900 Hz range)
- **Signal visualization** with waveform and spectrum displays
- **Adaptive threshold** with noise floor estimation

### 📡 Ham Radio Features
- **Automatic callsign detection** with validation against ITU regulations
- **QRZ.com integration** for instant operator information lookup
- **Callsign logging** with timestamp tracking
- **Interactive UI** with clickable callsigns for detailed info

### 📝 Technical Highlights
- **Goertzel algorithm** for efficient tone detection
- **Adaptive timing** for variable speed decoding
- **SNR calculation** with confidence metrics
- **Web Audio API** for real-time signal processing

## 🚀 Getting Started

### Prerequisites
- Modern web browser with microphone access
- QRZ.com account with XML data subscription (optional, for callsign lookups)

### Installation
1. Clone this repository:
   ```
   git clone [https://github.com/Sparks72/Morse-decoding-with-LLMs/QRZ-Intergration.git]
   ```
2. Open `index.html` in your web browser
3. Allow microphone access when prompted

### Using the Decoder

1. **Starting the Decoder**:
   - Click "Start Decoding" or press the spacebar
   - Adjust the threshold level if needed (recommended: 0.10)

2. **Decoding Morse Code**:
   - The application will automatically detect the frequency and speed
   - Watch the waveform and spectrum displays for signal visualization
   - Decoded text appears in the output window

3. **Using QRZ Integration**:
   - Enter your QRZ.com username and password
   - Click "Test QRZ Connection" to verify
   - Enable "Auto-detect callsigns" to automatically identify and lookup callsigns
   - Click on any highlighted callsign to view operator details

4. **Keyboard Shortcuts**:
   - **Spacebar**: Start/Stop decoding
   - **Ctrl+C**: Clear output

## ⚙️ Technical Details

### Morse Code Decoding Process
The application uses the following pipeline for decoding:
1. Audio capture using Web Audio API
2. Signal processing with Goertzel algorithm for tone detection
3. Threshold-based signal detection with adaptive noise floor estimation
4. Timing analysis for dot/dash determination
5. Morse pattern matching to alphanumeric characters
6. Automatic speed (WPM) adaptation based on dot length

### Callsign Detection
- Regular expression pattern matching with ITU regulation validation
- Contextual filtering to avoid false positives
- QRZ.com XML API integration for operator data

### Audio Processing Parameters
- **FFT Size**: 512 samples (optimized for responsiveness)
- **Frequency Range**: 500-900 Hz (configurable)
- **Speed Range**: 12-40 WPM (configurable)
- **Smoothing Time Constant**: 0.3 (balanced for stability)

## 🔧 Configuration Options

| Parameter | Description | Default |
|-----------|-------------|---------|
| Target Frequency | Center frequency for detection | 700 Hz |
| Speed (WPM) | Words per minute for manual timing | 20 WPM |
| Threshold Level | Signal detection threshold | 0.10 |
| Noise Reduction | Background noise filtering level | 5 |

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- [QRZ.com](https://www.qrz.com/) for providing the callsign database API
- Web Audio API for real-time audio processing capabilities
- The amateur radio community for ongoing testing and feedback

## 📧 Contact

Project Link: [https://github.com/Sparks72/Morse-decoding-with-LLMs/QRZ-Intergration)

---

*73's and happy decoding!*
