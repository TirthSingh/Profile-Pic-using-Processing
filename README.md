# Video Capture Sketch Effect

This project is a **Processing sketch** that uses the webcam to capture live video input and applies a pixelated sketch effect. By drawing larger "strokes" over pixels, it creates an artistic sketch-like representation of the video feed in real-time.

## Features

- Captures video from the default camera
- Applies a sketch effect by drawing points over pixels in steps
- Uses a large stroke weight to create a hand-drawn aesthetic
- Stops after one frame to capture a static "snapshot" look

## Requirements

- **Processing**: Ensure you have Processing installed.
- **Processing Video Library**: This project requires the `processing.video.*` library for video capture.

## Setup and Installation

1. Open Processing and install the Video library:
   - Go to `Sketch > Import Library > Add Library...`
   - Search for **Video** and install it.

2. Copy and paste the code into a new Processing sketch and run it.

## Code Overview

- **Capture Object Initialization**: The webcam is initialized and started with `Capture video`.
- **Capture Event**: Uses `captureEvent` to continuously update the video frames.
- **Sketch Effect**:
  - Loops over every 10th pixel horizontally and vertically for faster rendering.
  - Draws each point with a larger stroke to simulate a sketch effect.
  - Stops after capturing one frame with `noLoop()` to display a static image.
