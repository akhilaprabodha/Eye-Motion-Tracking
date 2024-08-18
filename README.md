# Eye Tracking Video Processing Script 🎥🔍

This repository contains a Python script that processes a video to detect and highlight the region of interest (ROI) around the eye. The script performs real-time video analysis, applying various image processing techniques to isolate and track eye movement.

<img src="https://github.com/akhilaprabodha/Eye-Motion-Tracking/blob/main/gifs_in_readme/eye_recording-ezgif.com-video-to-gif-converter.gif" width="100%">

## Features ✨

- `Grayscale Conversion:` Converts the region of interest (ROI) to grayscale for easier processing.
- `Gaussian Blur:` Applies a Gaussian blur to reduce noise and smooth the image.
- `Thresholding:` Uses thresholding to create a binary image, isolating the eye for contour detection.
- `Contour Detection:` Identifies and highlights the largest contour (presumed to be the eye) with bounding boxes and crosshairs.
- `Real-time Visualization:` Displays the processed video frames in real-time.

## Installation 📦

To run this script, you need to have Python installed along with the following dependencies:

```bash
pip install opencv-python numpy
```

## Usage 🚀

1. Clone the repository:
```bash
git clone https://github.com/akhilaprabodha/Eye-Motion-Tracking.git
cd Eye-Motion-Tracking
```

2. Run the script:

```bash
python eye_motion_tracking.py
```

3. Script Explanation:

- The script opens a video file (eye_recording.flv) or captures video from a camera.
- It defines the region of interest (ROI) within the video frame to focus on the eye.
- The ROI is processed through grayscale conversion, Gaussian blur, and thresholding.
- Contours are detected and the largest one is highlighted with a bounding box and crosshairs.
- The processed frames are displayed and saved as three separate output videos.

## Output Videos 🎬

**1. Thresholded Output 🔲**
- This video shows the thresholded version of the ROI, where the eye is isolated in a binary image.

<img src="https://github.com/akhilaprabodha/Eye-Tracking-System/blob/main/gifs_in_readme/output_threshold-ezgif.com-video-to-gif-converter.gif" width="100%">

**2. Grayscale ROI Output 🌑**
- This video displays the grayscale version of the ROI, which is used as the base for further processing.

<img src="https://github.com/akhilaprabodha/Eye-Tracking-System/blob/main/gifs_in_readme/output_gray_roi-ezgif.com-video-to-gif-converter.gif" width="100%">

**3. Contour Detection ROI Output 🎯**
- This video highlights the ROI with the detected contour, bounding box, and crosshairs.

<img src="https://github.com/akhilaprabodha/Eye-Tracking-System/blob/main/gifs_in_readme/output_roi-ezgif.com-video-to-gif-converter.gif" width="100%">

## Contributing 🤝
Contributions are welcome! If you have any improvements or additional features in mind, feel free to open a pull request.
