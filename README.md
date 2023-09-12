# Video Frame Extractor

## Introduction

This Python script is a simple tool for extracting frames from one or multiple video files using the OpenCV library and saving them into a file directory. It utilizes the `glob` module to locate all `.mp4` video files in the current directory as a starting point for extraction.

## Prerequisites

Before you can use this script, you need to have the following prerequisites installed:

- Python 3.x
- OpenCV (`opencv-python` package)
- `glob` module (usually included with Python)

You can install OpenCV via pip:

```bash
pip install opencv-python
```

## Usage

1. Copy the script provided into a Python file (e.g., `extractor.py`).

2. Place the video files you want to extract frames from (in `.mp4` format) in the same directory as the script.

3. Open a terminal or command prompt and navigate to the directory containing the script and video files.

4. Run the script:

```bash
extractor.py
```

5. The script will locate all `.mp4` files in the directory and proceed to extract frames from each video.

6. Extracted frames will be saved in a subdirectory with the same name as the video file, suffixed with `_frames`.

7. You can customize the script by modifying the extraction rate or file format as needed.

## Example

Here is how the script works using the provided code:

- It searches for all `.mp4` files in the current directory.
- For each video found, it opens the video file, extracts frames, and saves them in a subdirectory named after the video with `_frames` appended.
- The frames are saved as JPEG images with filenames like `frame0.jpg`, `frame1.jpg`, etc.

## Customization

You can customize this script to suit your specific requirements by modifying the following parameters:

- Frame extraction rate: To control how frequently frames are extracted, adjust the frame capture logic in the script.
- Output file format: You can change the output file format (currently set to JPEG) by modifying the filename in the `cv2.imwrite()` function.

