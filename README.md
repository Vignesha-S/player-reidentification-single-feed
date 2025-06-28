# Player Re-Identification in a Single Feed

## Overview
This project detects and tracks players in a football video using a YOLOv11 model and Deep SORT tracker. Each player is assigned a consistent ID, even when they go out of frame and return.

## Files
- `main.ipynb`: Colab notebook for detection + tracking
- `output_with_ids.mp4`: Output video with consistent player IDs
- `best.pt`: YOLOv11 model (provided)
- `15sec_input_720p.mp4`: Input video (provided)

## Setup
### Install Dependencies
```bash
pip install ultralytics
pip install opencv-python-headless
pip install deep_sort_realtime

## 🔗 Model Download

The YOLOv11 model file `best.pt` is not included in this repo due to size limits.  
You can download it from the link below and place it in the root folder or as needed:

👉 [Download best.pt from Google Drive](https://drive.google.com/file/d/1-5fOSHOSB9UXyP_enOoZNAMScrePVcMD/view)
