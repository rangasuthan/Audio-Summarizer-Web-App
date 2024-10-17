# Audio-Summarizer-Web-App
Flask-based web application that accepts audio files, transcribes them, and provides a text summary using a Hugging Face summarization model. The project demonstrates the integration of automatic speech recognition (ASR) and text summarization using state-of-the-art AI models.

# Audio Summarizer App

### Description
This project is a Flask-based web application that allows users to upload audio files, automatically transcribes the speech in the audio, and provides a concise summary of the transcription. The app leverages Google Speech Recognition for transcription and a Hugging Face summarization model to create a summary of the transcribed text. The audio is processed and handled in chunks to allow large files to be summarized as well.

### Features
- Upload audio in `.wav` or `.mp3` format.
- Automatically convert `.mp3` files to `.wav` if needed.
- Transcribes audio using Google Speech Recognition (with an offline fallback using CMU Sphinx).
- Summarizes the transcribed text using a Hugging Face BART model.
- Outputs both the transcription and the summary on the web interface.

### Tech Stack
- Flask (Python web framework)
- Hugging Face Transformers (for text summarization)
- Google Speech Recognition API (for audio transcription)
- Pocketsphinx (Offline transcription fallback)

### Requirements
Before running the application, ensure you have the following dependencies installed:

```bash
Flask==2.0.1
transformers==4.22.2
torch==2.0.1
speechrecognition==3.8.1
pydub==0.25.1
pocketsphinx==5.0.0
