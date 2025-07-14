# 🔍 Timestamp from Spoken Phrase

This project processes a video to find the exact timestamp where a given spoken phrase occurs using Whisper for transcription and RapidFuzz for fuzzy matching.

## 📂 Files

- `NnNVd1JpSW5jS1VfMzYwcA_out.mp4`: Source video file (automatically downloaded)
- `timestamp_from_speech.ipynb`: Notebook that runs the entire pipeline

## 🚀 How It Works

1. Downloads the video from a given URL.
2. Transcribes the audio using OpenAI Whisper with word-level timestamps.
3. Cleans and tokenizes the transcribed words.
4. Uses fuzzy matching (RapidFuzz) to search for the queried phrase in the transcript.
5. Returns the timestamp of the phrase’s first occurrence.

## 🧰 Requirements

All dependencies are installed within the Colab notebook:

- `openai-whisper`
- `rapidfuzz`
- `ffmpeg-python`

## ▶️ Usage

1. Run the notebook in Google Colab.
2. Provide your target spoken phrase as input.
3. The notebook will:
   - Transcribe the audio
   - Match your phrase
   - Print out the timestamp (in seconds and mm:ss format)

## 🕒 Output

Displays the time at which the queried phrase appears in the video.
