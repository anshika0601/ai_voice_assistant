
# 🎙️ AI Voice Assistant

An AI-powered **Voice Assistant** built with **Whisper (Speech-to-Text), Groq LLM, gTTS (Text-to-Speech), and Gradio**.  
It allows you to record speech 🎤, transcribe it into text 📝, generate a smart reply 💡, and listen to the response 🔊.

---

## 🚀 Features
- 🎤 **Speech-to-Text** using [OpenAI Whisper](https://github.com/openai/whisper) (`medium` model for better Hindi + English support).
- 💡 **AI Reply Generation** powered by [Groq LLM](https://groq.com/).
- 🔊 **Text-to-Speech** using [gTTS](https://pypi.org/project/gTTS/) (supports Hindi, English, and many languages).
- 🖥️ **Gradio UI** for an interactive experience with recording, transcription, and audio playback.
- 📜 Conversation display with user input and assistant reply.

---

## 🛠️ Tech Stack
- **STT** → Whisper (local, `medium` model)
- **LLM** → Groq via LangChain
- **TTS** → gTTS (Hindi by default)
- **UI** → Gradio

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/voice-assistant.git
cd voice-assistant

### 2️⃣ Install dependencies
Install the required Python packages using pip:
```bash
pip install openai-whisper groq gtts gradio langchain
```

### 3️⃣ Set up API key
Obtain your Groq API key from [Groq](https://groq.com/) and set it as an environment variable:
```bash
export GROQ_API_KEY='your_api_key_here'
```

### 4️⃣ Run the app
Launch the application:
```bash
python app.py
```


---
🌍 Language Support

Whisper → Multilingual transcription (but Hindi accents may need medium or large models for better accuracy).

gTTS → Supports 30+ languages including hi (Hindi) and en (English).

🔄 Possible Improvements

Use Coqui TTS or pyttsx3 for faster, offline TTS.

Switch to Streamlit UI for a cleaner dashboard.

Add multi-turn conversation history with LangChain memory.

Support real-time streaming audio (e.g., LiveKit or WebRTC).
