# 📡 Voice-Controlled IoT Automation System with AI-Powered Command Extraction and User Authentication

## 📌 Description:
Architected and implemented a voice-driven IoT automation system leveraging advanced speech and NLP models to interpret user commands and control smart home appliances. The system uses OpenAI’s Whisper for high-accuracy speech-to-text conversion, followed by a custom Named Entity Recognition (NER) module for extracting actionable entities such as appliance names and control operations (e.g., “switch on fan” → {appliance: fan, action: 1}).

A Flask-based backend exposes RESTful APIs that accept .wav audio inputs and return structured JSON responses. The system is designed for extensibility and real-time smart device interaction.

## 🧰 Key Technologies:
- Speech-to-Text: OpenAI Whisper (base)
- NLP: spaCy-based Custom NER
- Authentication: Voice recognition using SpeechBrain's ECAPA-TDNN model, combined with password verification
- Backend: Python Flask API
- Data Output: JSON-formatted commands
- Client Interfaces: Android app (MediaRecorder + OkHttp) and minimal frontend web app

## 📍 Current Status:
- Backend API is functional and tested via Postman for accurate transcription and NER-based intent parsing
- Voice authentication system implemented using SpeechBrain with combined password check
- Android app records and sends audio (currently refining API communication over Wi-Fi)
- Lightweight frontend web app in place for sending audio and receiving command outputs
- System returns appliance-control commands like { "appliance": "light", "action": 1 }

## 🌐 Future Applications:
- Integration with IoT microcontrollers (e.g., ESP32/Arduino) for real-world automation
- Multi-user support with voiceprint authentication
- Multilingual and contextual command understanding
- Full smart home automation platform with scheduled tasking and remote access
