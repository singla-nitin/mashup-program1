# Mashup Program

This program is designed to generate a mashup of YouTube videos from a specified singer by downloading, converting, trimming, and merging audio clips into one output file.

## Requirements

- Python 3.x
- Google YouTube Data API
- Libraries: `moviepy`, `yt-dlp`, `googleapiclient`, `dotenv`, `os`, `sys`
- FFmpeg (for handling video and audio processing)

## Features

1. **Download Videos**: Download N videos of a specific singer from YouTube.
2. **Convert to Audio**: Convert the downloaded videos to audio files.
3. **Trim Audio**: Cut the first Y seconds of the audio files.
4. **Merge Audio**: Merge all trimmed audios into one output file.

## How to Run

Run the program using the command line:

```bash
python <YourRollNumber>.py <SingerName> <NumberOfVideos> <AudioDuration> <OutputFileName>
```

### Example:

```bash
python 1015579.py "Sharry Maan" 20 20 1015579-output.mp3
```

### Arguments:

1. **SingerName**: The name of the singer (e.g., "Sharry Maan").
2. **NumberOfVideos**: Number of videos to download (N ≥ 10).
3. **AudioDuration**: Duration in seconds for trimming the audio (Y ≥ 20).
4. **OutputFileName**: Name of the final output file.

### Example Usage:

```bash
python 101556.py "Sharry Maan" 20 20 101556-output.mp3
```

## Input Validation

- The program checks for the correct number of parameters.
- It displays appropriate error messages for incorrect inputs.
- Handles exceptions where necessary.

## Setup and Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/singla-nitin/mashup-program1.git

   ```

2. Install the necessary dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the root directory and add your YouTube Data API key:

   ```
   API_KEY=your_youtube_api_key
   ```

## License

Author: Nitin Singla (Repo Owner)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to use, copy, modify, and distribute the Software, subject to the following conditions:
Attribution: Credit must be given to the original author (the repo owner), Nitin Singla, in any redistribution or reuse of this code.

Exclusion of Third-party Libraries: This license does not apply to any third-party libraries or packages included in the project. Those components are governed by their respective licenses and terms, which must be followed.

No Warranty: The software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement.
