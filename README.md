
# 🎙️ Voice-to-Voice GenAI Chatbot

A real-time voice-based chatbot powered by OpenAI's Whisper for speech-to-text, Groq's LLaMA3 model for AI-generated replies, and Google Text-to-Speech (gTTS) for converting text back to speech. Built with a clean Gradio interface for seamless user interaction.

## ✨ Features

- 🎧 Accepts audio input from microphone or file
- 🧠 Uses **Whisper** to transcribe audio to text
- 🤖 Sends the text to **Groq's LLaMA3 model** to generate a smart response
- 🔊 Converts the AI-generated text response back into speech with **gTTS**
- 🌐 Interactive UI built using **Gradio**

---

## 📁 Project Structure

```
├── app.py                # Main application script
├── requirements.txt      # Dependencies for setting up the environment
└── README.md             # Project documentation
```

---

## 🚀 How to Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/your-username/voice-to-voice-genai.git
cd voice-to-voice-genai
```

### 2. Create a virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Set your Groq API Key

Edit the `app.py` file and paste your Groq API key here:

```python
os.environ['GROQ_API_KEY'] = 'your_groq_api_key_here'
```

Or, alternatively, set it as an environment variable:

```bash
export GROQ_API_KEY=your_groq_api_key_here
```

---

## 🧠 Models Used

- [`whisper-base`](https://github.com/openai/whisper): For audio transcription
- [`llama3-8b-8192`](https://console.groq.com/): Hosted on Groq API
- [`gTTS`](https://pypi.org/project/gTTS/): Google Text-to-Speech engine

---

## 🖼️ Demo Interface

Once you launch the app, you’ll see a Gradio interface that allows:

- Uploading or recording your voice
- Getting real-time transcriptions and AI-generated replies
- Listening to the AI-generated voice response

---

## 🔧 Usage

```bash
python app.py
```

It will open a Gradio interface in your browser.

---

## 📌 Notes

- Ensure your device has a working microphone and speaker for best experience.
- Whisper’s transcription is done locally; Groq API is used for language generation.
- gTTS requires an internet connection to function.

---

## 📃 License

This project is open source under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

- [OpenAI Whisper](https://github.com/openai/whisper)
- [Groq API](https://console.groq.com/)
- [gTTS - Google Text to Speech](https://pypi.org/project/gTTS/)
- [Gradio](https://www.gradio.app/)

