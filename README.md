# Voice To Voice with LLM Response 

This app uses Whisper for speech recognition, Groq for generating chatbot responses, and gTTS for text-to-speech synthesis. Users can speak into the microphone, and the app will transcribe the speech, send it to a large language model (LLM) for a response, and then play the LLM’s response as speech.

**Features**

Speech Recognition: Convert spoken audio into text using Whisper.
Chatbot Responses: Get responses from an LLM powered by Groq.
Text-to-Speech: Convert the chatbot's response into speech using Google Text-to-Speech (gTTS).
Real-time Interaction: The app supports real-time voice-based interaction using Gradio.

**Requirements**
Python 3.x
Gradio
Whisper
gTTS
Groq Python client

Setup
>pip install gradio whisper gtts groq
>
>
