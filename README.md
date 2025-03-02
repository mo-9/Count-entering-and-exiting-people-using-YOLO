# People Detection and Counting using YOLOv8

This project detects and tracks people in a video using **YOLOv8** and **object tracking** techniques. It counts people entering and exiting specific areas.

## Features
- **YOLOv8-based Object Detection**
- **Object Tracking** using a custom tracker
- **People Counting** in defined areas
- **Saves Processed Video Output**

## Installation
### 1. Clone the Repository
```bash
git clone https://github.com/mo-9/Count-entering-and-exiting-people-using-YOLO.git
cd Count-entering-and-exiting-people-using-YOLO
```

### 2. Install Dependencies
Ensure you have Python 3.9+ installed, then run:
```bash
pip install -r requirements.txt
```

### 3. Download YOLOv8 Model
```bash
wget https://github.com/ultralytics/assets/releases/download/v8/yolov8n.pt
```

## Usage
### 1. Run the Script
```bash
python detect.py
```

### 2. Input Video
Ensure you have a video file (e.g., `peoplecount1.mp4`) in the project folder.

### 3. Output Video
After running, check `output.mp4` in the project folder.

## Troubleshooting
- **Video not saving?** Ensure `cv2.VideoWriter` size matches resized frame.
- **Empty output video?** Try playing with VLC or run:
  ```bash
  ffmpeg -i output.mp4 -c:v copy fixed_output.mp4
  ```
- **CUDA issues?** Ensure PyTorch and Ultralytics support your GPU.

## Contributing
Pull requests are welcome! Please open an issue for bug reports or feature requests.

## License
MIT License

