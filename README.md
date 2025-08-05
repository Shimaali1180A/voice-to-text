# 🎙️ Voice-to-Text & GPT Response System

This project allows you to:
1. Record your voice using a microphone,
2. Transcribe the audio into text using OpenAI’s Whisper API,
3. Generate an AI-based reply using OpenAI’s GPT model,
4. And finally, convert the reply into speech (Text-to-Speech) and play it aloud.

It’s built in Python and is perfect for experimenting with voice-enabled AI interactions.

---

## 📁 Project Structure

voice_1/
├── record_to_text.py       # Records audio and saves it as a .wav file
├── generate_reply.py       # Transcribes audio, generates a GPT reply, and plays it as speech
├── my_recording.wav        # Example recorded audio file

---

## 🧠 Features

- 🎤 Audio Recording: Capture live voice from the microphone.
- ✨ Speech-to-Text: Transcribe audio using OpenAI Whisper (`whisper-1` model).
- 🤖 AI Response: Generate an intelligent response with GPT-3.5-Turbo.
- 🔊 Text-to-Speech: Convert the GPT-generated reply into audible speech using pyttsx3.

---

## ⚙️ Requirements

- Python 3.8+
- openai (Python SDK)
- sounddevice
- scipy
- pyttsx3 (for text-to-speech)

### Install required packages:

```bash
pip install openai sounddevice scipy pyttsx3

🔑 API Key

To use OpenAI services, set your API key in your Python code like this:

from openai import OpenAI

client = OpenAI(api_key="your_openai_api_key_here")

💡 Make sure you have sufficient quota/balance in your OpenAI account.

🔒 Do NOT share your API key publicly or upload it to GitHub.
Use environment variables or .env files to secure your credentials.

📝 How to Use

1. Record Your Voice

Run this script to record audio from your microphone:

python record_to_text.py

This will create a file named my_recording.wav.

2. Transcribe, Generate Reply, and Play Response

Then run:

python generate_reply.py

This script:
 • Transcribes your recorded voice using Whisper API.
 • Generates a response using GPT-3.5-Turbo.
 • Displays both the transcription and the response.
 • Reads the GPT response out loud using Text-to-Speech.

📌 Example Output

🎤 Transcribed Text:
Hello, how are you?

🤖 GPT Reply:
I'm doing well, thank you! How can I help you today?

🔊 Speaking...
(You will hear the response read aloud)

📦 Notes
 • This project uses OpenAI’s paid APIs — make sure you have an active balance.
 • Audio files are stored locally in .wav format.
 • You can edit the scripts to customize the recording time or speech rate.

🔐 Security Reminder

Your OpenAI API key is sensitive information. Never push your key to GitHub repositories.
Use .gitignore to exclude files that contain keys, and consider using environment variables for better security.

📜 License

MIT License – free to use, modify, and share with attribution.
