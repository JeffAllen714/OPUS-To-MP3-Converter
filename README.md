# Opus to MP3 Converter

This is a Python application with a graphical user interface (GUI) that allows users to convert Opus audio files to MP3 format. It uses FFmpeg for the conversion process and provides a simple, user-friendly interface for batch conversion of Opus files.

## Features

- Convert individual Opus files to MP3 format
- Batch convert all Opus files in a selected folder
- User-friendly GUI built with PyQt6
- Progress bar to show conversion status
- Multithreaded conversion for improved performance

## Requirements

- Python 3.6+
- PyQt6
- FFmpeg

## Installation

1. Clone this repository or download the source code.

2. Install the required Python packages:

   ```
   pip install PyQt6
   ```

3. Install FFmpeg:
   - On Windows: Download from [ffmpeg.org](https://ffmpeg.org/download.html) and add it to your PATH.
   - On macOS: Use Homebrew: `brew install ffmpeg`
   - On Linux: Use your distribution's package manager, e.g., `sudo apt-get install ffmpeg`

## Usage

1. Run the script:

   ```
   python opus_to_mp3_converter.py
   ```

2. In the GUI:
   - Click "Input Folder" to select the folder containing your Opus files.
   - Click "Output Folder" to choose where the converted MP3 files will be saved.
   - Click "Convert" to start the conversion process.

3. The progress bar will show the conversion progress, and the log window will display details about the conversion process.

## How it Works

The application uses FFmpeg to convert Opus files to MP3 format. It processes files in parallel using Python's `ThreadPoolExecutor` to improve performance. The GUI is built using PyQt6, providing a responsive interface for users.

## Contributing

Contributions to improve the converter are welcome. Please feel free to submit a Pull Request.

## Disclaimer

This tool is for personal use only. Ensure you have the right to convert and use the audio files.
