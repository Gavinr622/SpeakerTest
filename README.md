# 🎧 Speaker / Headphone Channel Test

A Python CLI tool that tests whether both channels of your speakers or headphones are working. It plays a tone in a random channel (Left or Right), and you have to identify which one — just like a hearing test, but for your audio gear.

Text-to-speech guides you through every step using your system's natural voice (Microsoft Zira or David on Windows).

---

## ✨ Features

- 🔊 Plays tones in the **left or right channel only**
- 🗣️ **Text-to-speech** intro, feedback, and results (uses Windows Zira/David voice)
- 🎵 Four different frequencies to keep rounds varied
- 🏆 Score summary at the end with a spoken verdict
- ⚙️ Configurable number of rounds

---

## 📦 Requirements

- Python 3.7+
- Windows, macOS, or Linux

Install dependencies:

```bash
pip install pyttsx3 sounddevice numpy
```

---

## 🚀 Usage

```bash
# Default — 5 rounds
python speaker_test.py

# Custom number of rounds
python speaker_test.py 10
```

---

## 🎮 How It Works

1. The script speaks the instructions aloud
2. Each round, it picks a random channel (left or right) and a random tone
3. You type `L` or `R` and press Enter
4. It tells you if you were right — both in text and speech
5. At the end, you get a score and a spoken summary

---

## 🪟 Voice Notes (Windows)

The script automatically picks the best available voice in this order:

| Voice | Gender | Style |
|-------|--------|-------|
| Microsoft Zira | Female | Natural, clear |
| Microsoft David | Male | Natural, clear |
| Microsoft Mark | Male | Fallback |

These are the same voices used by Windows phone assistants and accessibility tools. If none are found, it falls back to the system default.

To install more voices on Windows:
**Settings → Time & Language → Speech → Add voices**

---

## 🛠️ Troubleshooting

| Problem | Fix |
|---------|-----|
| One channel silent | Check OS audio balance (Settings → Sound → Balance) |
| No sound at all | Make sure your device is set as the default output |
| TTS not speaking | Run `pip install --upgrade pyttsx3` |
| `sounddevice` error | Try `pip install --upgrade sounddevice` |

---

## 📁 Project Structure

```
speaker-test/
├── speaker_test.py   # Main script
└── README.md         # This file
```

---

## 📄 License

MIT — free to use, modify, and share.
