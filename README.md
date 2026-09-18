# 🎧 SpeakerTest

**SpeakerTest** is a desktop audio testing application for Windows that helps you test your left and right audio channels, configure tones, and optionally use text-to-speech narration.

## ✨ Features

* 🎧 Left and right speaker/channel testing
* 🔊 Adjustable tone volume
* 🎵 Adjustable tone duration
* ⏱️ Configurable countdown
* 🗣️ Text-to-speech narration
* 🎚️ Adjustable voice speed
* 👤 Multiple voice options
* ↩️ Reset Voice settings
* 🎨 Multiple UI themes

  * Dark
  * Light
  * Midnight
  * Sunset
  * Forest
* 🔐 Sign In
* 📝 Create Account
* 👤 Guest mode
* 📊 Test history
* 👤 User profile
* 🏆 Test results
* 💬 Discord community button
* ✕ Quit test button
* ☁️ Cloudflare Workers + D1 backend

## 🖥️ Requirements

SpeakerTest is designed for **Windows**.

You need:

* Windows 10 or newer
* A working audio output device
* Python 3.10+ if running from source

## 🚀 Running From Source

Clone the repository:

```bash
git clone YOUR_REPOSITORY_URL
cd SpeakerTest
```

Install the dependencies:

```bash
py -m pip install -r requirements.txt
```

Run the application:

```bash
py app.py
```

## 📦 Building the EXE

The repository includes `build.bat`.

Simply run:

```text
build.bat
```

The finished application will be created at:

```text
dist\SpeakerTest.exe
```

You can then run `SpeakerTest.exe` without manually launching Python.

## 🔊 Audio Testing

SpeakerTest generates audio separately for the left and right channels.

**Important:** Some computers, headphones, Bluetooth devices, audio drivers, or Windows audio settings can mix stereo audio into both channels. If both sides play the same tone, check your Windows audio configuration and the output device.

## 🗣️ Voice

SpeakerTest includes optional text-to-speech narration.

Voice settings include:

* Enable/disable narration
* Voice selection
* Voice speed
* Test Voice
* Reset Voice

The available voices depend partly on the voices installed on the computer.

## 🎨 Themes

The application includes five themes:

| Theme    | Description               |
| -------- | ------------------------- |
| Dark     | Standard dark interface   |
| Light    | Light interface           |
| Midnight | Dark blue-style interface |
| Sunset   | Warm-colored interface    |
| Forest   | Green-themed interface    |

## ☁️ Backend

SpeakerTest uses a Cloudflare backend for account and application data.

The backend uses:

* Cloudflare Workers
* Cloudflare D1
* API authentication
* Password hashing
* User settings
* Test history

The desktop application communicates with the backend over HTTPS.

## 🔐 Privacy

Do not put passwords, API keys, private tokens, or other secrets into the source code before publishing this project.

If you fork this project, review the API configuration and backend settings before deploying your own version.

## 💻 Project Structure

```text
SpeakerTest/
│
├── app.py
├── README.md
├── requirements.txt
├── build.bat
│
└── assets/
```

## 🐛 Reporting Bugs

If you find a bug, please open a GitHub Issue and include:

1. Windows version
2. Speaker/headphone device
3. SpeakerTest version
4. What you were doing
5. What happened
6. Any error message

Please remove private information from logs before posting them.

## 📜 License

Choose a license for your repository before publishing the project.

## 👨‍💻 Author

**Gavin Codeworks**

Built with Python, PyQt6, NumPy, SoundDevice, pyttsx3, Cloudflare Workers, and Cloudflare D1.

---

⭐ If you find SpeakerTest useful, consider starring the repository!
