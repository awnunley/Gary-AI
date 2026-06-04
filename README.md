# Gary-AI

Gary is an interactive, voice-activated AI assistant built for the Raspberry Pi. Powered by the Gemini API for intelligence and Google Cloud Text-to-Speech for natural voice responses, Gary listens for his wake word, processes commands, and provides vocal feedback. The project also features integrated WS2812B (NeoPixel) LED status indicators to visually show when Gary is listening, processing, or speaking.

## 🚀 Features

* **Custom Wake Word Detection:** Local, low-latency wake word detection ("Gary") using Picovoice Porcupine.
* **Advanced AI Reasoning:** Powered by Google's `gemini-1.5-pro` model with a personalized, helpful persona.
* **Natural Speech Synthesis:** High-quality voice output using Google Cloud Text-to-Speech (Wavenet).
* **Visual Feedback (Optional):** Dynamic LED strip patterns (WS2812B) to indicate assistant states (Listening, Processing, Speaking).
* **Headless Operation:** Configured to run automatically on system boot using a Linux `systemd` service.

---

## 🛠️ Hardware Requirements

* Raspberry Pi (Model 4B or similar recommended)
* USB Microphone or Microphone Array (e.g., ReSpeaker)
* External Speaker (connected via 3.5mm jack, USB, or HDMI)
* *Optional:* WS2812B (NeoPixel) LED Strip (connected to GPIO 18)
* Stable 5V Power Supply

---

## 💻 Software Prerequisites

Before installing the Python dependencies, ensure your Raspberry Pi system packages are up to date and required build tools are installed:

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install scons build-essential python3-dev alsa-utils -y
