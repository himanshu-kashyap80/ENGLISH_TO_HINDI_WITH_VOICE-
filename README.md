# English to Hindi Translator (with Voice Input & Output)
**Project:** English-to-Hindi Translator for Government Websites  
**Includes:** Flask backend, improved GUI, voice input (Speech-to-Text) and voice output (Text-to-Speech)

## Features
- Speak English using your microphone and have it transcribed into text (Web Speech API).
- Click **Translate** to send text to the Flask backend which uses `googletrans` for translation.
- Listen to the Hindi translation via the browser's SpeechSynthesis API.
- Simple, government-appropriate UI: clean layout, responsive, accessible buttons, loader.

## Requirements
- Python 3.10+ recommended
- Microphone access in your browser
- Modern browser (Chrome/Edge recommended) for reliable Web Speech API support

## Setup (local)
1. Clone or extract this project.
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate    # macOS / Linux
   venv\Scripts\activate     # Windows (PowerShell)
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the app:
   ```bash
   python app.py
   ```
5. Open http://127.0.0.1:5000 in your browser.

## Notes & Tips
- The Web Speech API (speech recognition) is currently best supported in Chrome/Edge on desktop.
- If you want offline or production-grade translation, replace `googletrans` with an official translation API (Google Cloud Translate, Microsoft Translator) and secure the API key on the server.

## Project structure
english_to_hindi_translator_with_voice/
├─ app.py
├─ requirements.txt
├─ templates/
│  └─ index.html
├─ static/
│  ├─ css/
│  │  └─ style.css
│  └─ js/
│     └─ main.js
└─ README.md

