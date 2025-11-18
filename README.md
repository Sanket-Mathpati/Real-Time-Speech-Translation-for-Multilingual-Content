# Speech to Speech Translator - (Modules 1–4)

A comprehensive multi-module project for **Speech Translation** workflows, covering environment setup, batch processing, and a full web-based user interface.

## ✨ Features

This monorepo is divided into four modules, built primarily with **Python** and a **Flask** web application.

| Module | Focus | Key Functionality |
| :--- | :--- | :--- |
| **Module 1** | **Environment Check** | Verify Python/audio stack, dependencies (`requirements.txt`), and quick sanity checks. |
| **Module 2** | **Batch Translation** | Offline toolkit for dataset preparation, converting audio formats (`mp3 ↔ wav`), and batch translation. |
| **Module 3** | **Realtime (Scripted)** | Command-line experiments for direct, real-time translation from mic/stream inputs. |
| **Module 4** | **Flask Web App (UI)** | Web interface for **Live Mic Translation**, **Audio/Video Uploads**, and **YouTube link translation** (with chunking and TTS output). |

### Supported Languages (UI)

The Flask web app supports translation to: `en`, `hi`, `pa`, `mr`, `kn`, `te`, `ta`, `gu`, `ml`, `bn`, `or`, and `ur`.

---

## 🚀 Quick Start (Module 4 - Web App)

The quickest way to get started is by running the Flask web application.

### 1. Prerequisites

* **Python 3.11–3.13** is recommended.
* **FFmpeg** is required for audio processing (automatically handled in Module 4 for Windows, but system-wide install is recommended for others).

### 2. Run the App

# Install dependencies for Module 4
cd speech-translator/module4
python -m pip install -r requirements.txt

# Run the application
python app.py

[http://127.0.0.1:5000](http://127.0.0.1:5000)
Module-Specific Commands
Module	Purpose	Example Command
Module 2	Batch Translate	python module2_batch_translator.py
Module 2	Convert MP3 to WAV	python convert_mp3_to_wav.py
Module 3	Run Realtime Script	python module3_ott_realtime.py

📝 License & Acknowledgments
This repository is provided for educational and research purposes under the MIT License.

Key Libraries Used: Python SpeechRecognition, Flask, gTTS, Edge TTS, librosa, moviepy, yt-dlp, and pytube.
