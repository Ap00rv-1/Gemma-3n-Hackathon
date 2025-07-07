# Gemma-3n-Hackathon
Google Hackathon on Gemma 3-n model.
AI Counsellor for Mental Health

This project aims to develop an AI-powered mental health counsellor that can hold emotionally intelligent conversations with users. The system combines speech recognition, emotion detection, LLMs (Gemma 3n), and text-to-speech synthesis to deliver supportive, empathetic interactions.

Speech-to-Text Recognition
Converts real-time voice input from users into text using Gemma 3n speech to text

Emotion Detection (In Progress)
Classifies emotional tone of the user’s voice using pretrained models (e.g., wav2vec2-based emotion recognition).

LLM-Based Response Generation
Uses Gemma 3n to generate contextual, empathetic responses based on the user's emotional state and input history.

Text-to-Speech Conversion (In Progress)
Converts generated text responses into natural-sounding speech using models like Microsoft's SpeechT5 or XTTS.

Dynamic Conversational Flow
User queries are stored in stacks, and conversations are mapped using graphs to track topics and emotional shifts. This allows Gemma 3n to tailor its tone and advice dynamically over time.

The AI Counsellor will serve as a non-judgmental, always-available support system for users to express their feelings. It will track emotional patterns over time, gently guide conversations, and provide personalized, affirming dialogue using Gemma 3n’s capabilities.




These are available datasets and model that we would like to use:
Datasources:
Datasets:

https://paperswithcode.com/dataset/lssed : copyright database, LSSED

TESS: https://tspace.library.utoronto.ca/handle/1807/24487 (Final)
https://www.kaggle.com/datasets/ejlok1/toronto-emotional-speech-set-tess

RAVDESS
https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio

SAVEE
https://www.kaggle.com/datasets/ejlok1/surrey-audiovisual-expressed-emotion-savee

Credma-D
https://www.kaggle.com/datasets/ejlok1/cremad

PreTrained Models:

For speech emotion recognition:
https://huggingface.co/ehcalabres/wav2vec2-lg-xlsr-en-speech-emotion-recognition
https://huggingface.co/speechbrain/emotion-recognition-wav2vec2-IEMOCAP

For speech to text:(Gemma 3n will be used here)
https://huggingface.co/openai/whisper-large-v3

For text to speech:(here also we will use gemma 3n)
https://huggingface.co/microsoft/speecht5_tts?text=I
https://docs.coqui.ai/en/latest/models/xtts.html#training

For LLM:(Gemma 3n could me used for SLM)
https://huggingface.co/facebook/blenderbot-400M-distill?text=I%27m+really+sad


Folder Structure (Planned)
ai-counsellor/
│
├── data/                   # Sample audio and emotion datasets
├── models/                 # Pretrained models (local/cache)
├── src/
│   ├── speech_to_text.py   # Converts voice to text
│   ├── emotion_detect.py   # Classifies user emotion
│   ├── response_gen.py     # Uses Gemma 3n to generate replies
│   ├── tts.py              # Text-to-speech converter
│   ├── memory.py           # Stack & graph-based memory
│   └── main.py             # Execution script
├── README.md
└── requirements.txt



🤝 Acknowledgements
Gemma 3n by Google

Hugging Face
