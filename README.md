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

**Setup**

1. Clone or download this repository.

2.Install the required dependencies:

```bash
pip install gradio whisper gtts groq```


3.Set up your Groq API Key:

-Get your Groq API key and save it as an environment variable.
-In the script, you can set the key directly or load it from a .env file:

```bash
export GROQ_API_KEY="your_api_key_here"

4.(Optional) Download the Whisper model you want to use. In the script, it loads the "base" model, but you can change it to other available models (e.g., "small", "medium", etc.).


**Usage**

1.Launch the app:

```bash
python app.py

2.The Gradio interface will open in your browser. You can speak into the microphone or upload an audio file.

3.The app will transcribe your speech, send it to the Groq API for a response, and play the response as speech.

**Example Interaction**

1.User: "What's the weather like today?"
2.App:
-Transcribes speech: "What's the weather like today?"
-Sends query to Groq: "What's the weather like today?"
-Groq responds: "Today's weather is sunny with a high of 75°F."
-Converts response to speech and plays it.


**Code Explanation**

-Whisper: Used to transcribe spoken audio into text.
-Groq: A large language model (LLM) that generates responses to user input.
-gTTS: Converts the text response from Groq into audio, which is then played back.
-Gradio: Provides an interactive interface for users to interact with the chatbot via audio input and output.


**Notes**
-Ensure you have a stable internet connection to interact with the Groq API.
-Adjust the Whisper model as needed depending on the desired accuracy and performance.


**License**
This project is licensed under the MIT License - see the LICENSE file for details.
