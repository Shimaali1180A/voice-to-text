# Voice-to-text 🎙️🤖

This project is a simple voice-based assistant that allows you to speak into a microphone, have your speech transcribed to text using OpenAI Whisper, generate a response using GPT-3.5, and read the response out loud.

---

## 📌 Features

- 🎤 **Voice Recording** – Capture audio from your microphone.
- 📝 project is a simple– Transcribe the recorded audio using OpenAI Whisper API.
- 💬 voice-based assis– Send the transcribed text to GPT and receive a reply.
- 🔊le voice-based assis– The reply is read out loud using built-in TTS.

---

## 🧰 Technologies Used

- Python
- [OpenAI API](https://platform.openai.com/)
-our speechlibrary versionce AI Assi-# Voice-to-Voic
# Voice-to-Voice AI– For recording
- AI Assista– For speech output (TTS)

---

## 📂 Project Structure

voice_1/
│
├── record_to_text.py         # Records audio and saves it as my_recording.wav
├── generate_reply.py         # Converts audio to text, gets GPT reply, and reads it aloud
├── my_recording.wav          # The recorded audio file
└── README.md                 # Project documentation

---

## 🛠️ Installation

Make sure you have Python 3.8+ installed.

1..
- 💬 **GPT Response** – 
```bash
git clone https://github.com/yourusername/voice_1.git
cd voice_1

 2. Install dependencies

pip install openai==1.97.1 sounddevice scipy pyttsx3

🔑 OpenAI API Key

Create an account at OpenAI, (https://platform.openai.com/) go to the API section, and generate a secret key.

In generate_reply.py, replace:

client = OpenAI(api_key="your_api_key_here")

with your actual key.

▶️ How to Use

1. Record Your Voice

python record_to_text.py

You’ll be prompted to start speaking. Your voice will be saved as my_recording.wav.

2. Transcribe and Generate a Response

python generate_reply.py

This script will:
 • Transcribe your audio
 • Send it to GPT
 • Print the GPT reply
 • Read the reply out loud

💡 Example

You say:

 “Hello, what can you do?”

Assistant replies (text + audio):

 “Hi there! I can listen to your voice, convert it to text, and answer using AI.”

📌 Notes
 • Make sure your OpenAI account has active credits or a billing method added.
 • The transcription accuracy may vary depending on background noise and pronunciation.
 • You can adjust the recording duration and voice settings in the code.

📞 Contact

For questions or suggestions, feel free to open an issue or contact me.
