# LibriSpeech Transcription Project

This project transcribes audio files from the LibriSpeech dataset using the Wav2Vec2 model from Facebook AI Research.

## Setup

1. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Project Structure

- `transcribe.py`: Main script for transcribing audio files
- `requirements.txt`: Project dependencies
- `LibriSpeech/`: Directory containing the audio files
- `transcriptions.json`: Output file containing the transcriptions

## Usage

1. Place your LibriSpeech audio files in the `LibriSpeech` directory
2. Run the transcription script:
```bash
python transcribe.py
```

The script will:
- Process all .flac files in the LibriSpeech directory
- Generate transcriptions using the Wav2Vec2 model
- Save the results to `transcriptions.json`

## Notes

- The Wav2Vec2 model expects audio files to be 16kHz
- The script will skip files that don't meet this requirement
- Progress and any errors will be printed to the console 