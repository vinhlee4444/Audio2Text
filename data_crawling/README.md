# Audio2Text Data Crawling Project

This project processes YouTube videos to extract audio and text data for audio-to-text alignment using Whisper.

## Features

- Download YouTube video subtitles
- Convert audio to WAV format
- Use Whisper for audio transcription with word-level timestamps
- Split audio into segments with aligned text
- Generate training data for audio-to-text models

## Dependencies

- Python 3.12.11
- whisper
- librosa
- pydub
- selenium
- yt-dlp
- requests
- beautifulsoup4
- matplotlib
- pandas

## Usage

1. Add YouTube URLs to `urls.txt`
2. Run the notebook cells in order:
   - Download subtitles
   - Process audio files
   - Generate word-level alignments
   - Split into training segments

## Output Structure

```
output_segments_grouped/
├── [audio_file_name]/
│   ├── 00.wav, 00.json, 00.txt
│   ├── 01.wav, 01.json, 01.txt
│   └── ...
```

## Note

Large audio files and output directories are excluded from Git tracking via `.gitignore`.