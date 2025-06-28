# Report: Player Re-Identification in a Single Feed

## 🎯 Objective
To track and consistently re-identify football players in a single video feed using object detection and tracking methods.

## 🧠 Approach & Methodology

1. **Detection**
   - Used the provided YOLOv11 model (`best.pt`) trained on player and ball detection.
   - Detected players (class 0) in each frame using the Ultralytics YOLO inference API.

2. **Tracking**
   - Integrated **Deep SORT** to maintain consistent player IDs across frames.
   - Tracked players even when they temporarily went out of frame.
   - Bounding boxes and IDs were overlaid on each frame and saved to video.

3. **Video Output**
   - Processed video saved as `output_with_ids.mp4` showing ID consistency.

## 🧪 Techniques Tried

- Baseline YOLO-only detection → worked for drawing bounding boxes but **no ID continuity**
- Deep SORT integration → **solved re-identification**
  - Used motion + bounding box data
  - Explored tweaking `max_age` and `n_init` parameters for stable IDs

## ⚠️ Challenges Faced

- Ensuring players are matched back correctly when overlapping
- Handling occasional ID switching when detections were briefly missed
- Colab memory and video I/O time limits

## 🔧 Remaining / Improvements

If given more time, I would:
- Add **appearance feature extraction** (e.g., color histograms, embeddings)
- Handle **occlusion** and **crowded player regions** more robustly
- Smooth tracking with **Kalman filtering + interpolation**
- Try Option 1 (multi-camera player mapping)

## ✅ Outcome

- Players were consistently re-identified in the single video feed.
- IDs were retained when players left and re-entered the frame.

