# Morse decoding with LLM's

This project is a fully browser-based Morse code decoder designed to work reliably in noisy conditions, without producing spurious characters. It operates entirely within modern browsers across platforms (Windows, Linux, MacOS), requiring no installation or dependencies.

## Features

- Real-time decoding of Morse code via microphone input
- Self-adjusting speed detection (12â€“40 WPM)
- Goertzel algorithm-based tone detection (500â€“900 Hz)
- Noise-adaptive thresholding to minimise false decoding
- Responsive visual feedback (waveform, spectrum, SNR)
- Fully self-contained HTML+JavaScript
- Works offline after initial load
- Compatible with all major browsers

## Getting Started

1. Open `index.html` in your browser.
2. Click **Start Decoding** and allow microphone access.
3. Tune your signal to the target frequency and observe the output.

## Publishing to GitHub Pages

1. Create a repository named `Morse decoding with LLM's`.
2. Upload these files.
3. Go to **Settings â†’ Pages** and set the source to the `main` branch and `/ (root)` directory.
4. Your decoder will be live at `https://<your-username>.github.io/morse-decoding-with-llms/`.

## License

This project is provided for educational and amateur radio use. Attribution appreciated.
