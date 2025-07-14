# 🌄 Panorama from Video

This project extracts frames from a rotating video and stitches them into a single panoramic image using OpenCV.

## 📂 Files

- `video.mp4`: Source video file (automatically downloaded)
- `panorama.jpg`: Final panorama image generated from the video

## 🚀 How It Works

1. Downloads the video from a given URL.
2. Extracts every 10th frame from the video and resizes them.
3. Uses OpenCV’s `Stitcher_create()` to stitch the selected frames into a panorama.
4. Displays and saves the final panorama image.

## 🧰 Requirements

All required libraries are handled within the Colab notebook:

- `opencv-python`
- `numpy`
- `matplotlib`

## ▶️ Usage

1. Run the notebook in Google Colab.
2. It will:
   - Download the video
   - Process and stitch the frames
   - Display the panorama
   - Offer a download link for the final image

## 🖼️ Output

A stitched panoramic image showing the full captured scene.
