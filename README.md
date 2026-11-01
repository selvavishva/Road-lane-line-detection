# 🚗 Road Lane Localization Using OpenCV

<p align="center">
  <b>A Computer Vision-Based Lane Detection System for Road Safety and Autonomous Driving Assistance</b>
</p>

---

## 📌 Project Overview

**Road Lane Localization** is a computer vision-based project developed using Python and OpenCV to detect and localize lane markings from road images and video streams.

The system processes video frames, identifies lane boundaries, and overlays the detected lane lines onto the original road footage. This project demonstrates fundamental computer vision techniques that can support autonomous driving and lane departure warning systems.

## 🎯 Objectives

- Detect road lane markings under different lighting and weather conditions.
- Perform video frame processing for lane detection.
- Identify lane boundaries and road direction.
- Improve detection under challenging road conditions such as shadows, sharp turns, and faded lane markings.
- Explore perspective transformation and thresholding techniques.
- Provide a foundation for autonomous driving assistance systems.

## 🧠 Abstract

Lane detection is an important component of autonomous driving systems, as it provides essential road information for vehicle navigation and safety.

This project implements a lane localization system using classical computer vision techniques, including:

- Canny Edge Detection
- Hough Transform
- Perspective Transformation
- Image Thresholding
- Region of Interest (ROI) Masking
- Camera Calibration

The system identifies lane markings from road images or video streams and overlays the detected lane boundaries onto the original frames.

## ⚙️ System Architecture

The project follows the following image and video processing pipeline:

```text
Input Image / Video
        |
        ▼
Camera Calibration
        |
        ▼
Perspective Transformation
        |
        ▼
Image Thresholding
        |
        ▼
Edge Detection (Canny)
        |
        ▼
Region of Interest (ROI)
        |
        ▼
Lane Line Detection
        |
        ▼
Lane Overlay
        |
        ▼
Display / Save Output Video
```

## 🔍 Existing System

The existing lane detection approach uses classical computer vision techniques:

- Canny Edge Detection for identifying edges.
- Hough Transform for detecting lane lines.
- Region of Interest (ROI) masking to focus on road regions.
- Frame-by-frame video processing.

### Limitations

- Limited adaptability to complex road conditions.
- Difficulty detecting faded or unclear lane markings.
- Sensitivity to lighting variations and shadows.
- Limited contextual understanding of surrounding traffic.
- Challenges in detecting lanes on sharp curves.

## 🚀 Proposed Enhancements

The following improvements can enhance the system's performance:

- Adaptive thresholding for improved lane detection.
- Lane direction and curvature detection.
- Better handling of challenging lighting conditions.
- Improved lane localization accuracy.
- Traffic condition analysis as a future enhancement.

## 🧰 Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| OpenCV | Image and video processing |
| NumPy | Numerical computations |
| MoviePy | Video processing |
| Matplotlib | Data visualization |
| Jupyter Notebook | Development and experimentation |

## 📂 Project Structure

```text
Road-Lane-Line-Detection/
│
├── camera_cal/
│
├── CameraCalibration.py
├── Thresholding.py
├── PerspectiveTransformation.py
├── LaneLines.py
├── main.py
│
├── Road_Lane_Line_Detection.ipynb
├── challenge_video.mp4
├── output.mp4
│
└── README.md
```

## 💻 System Requirements

### Software Requirements

- Python 3.x
- Jupyter Notebook
- OpenCV
- NumPy
- Matplotlib
- MoviePy
- Docopt

### Hardware Requirements

- Multi-core processor
- Minimum 8 GB RAM recommended
- Camera or video input for lane detection

## ▶️ Installation and Execution

### 1. Clone the Repository

```bash
git clone https://github.com/selvavishva/Road-lane-line-detection.git
```

### 2. Navigate to the Project Directory

```bash
cd Road-lane-line-detection
```

### 3. Install Dependencies

```bash
pip install opencv-python numpy matplotlib moviepy docopt
```

### 4. Run the Project

```bash
python main.py
```

Alternatively, open the Jupyter Notebook:

```bash
jupyter notebook Road_Lane_Line_Detection.ipynb
```

### 5. Output

- **Input:** Road video (`challenge_video.mp4`)
- **Output:** Processed video with detected lane markings (`output.mp4`)

## 🔬 Methodology

The system follows these image processing steps:

1. **Grayscale Conversion:** Converts the input image into grayscale.
2. **Gaussian Blur:** Reduces image noise and unwanted details.
3. **Canny Edge Detection:** Identifies important edges in the road image.
4. **ROI Masking:** Focuses processing on the relevant road region.
5. **Hough Transform:** Detects lane line segments.
6. **Perspective Transformation:** Converts the road view into a bird's-eye perspective.
7. **Lane Detection:** Identifies and localizes lane boundaries.
8. **Lane Overlay:** Projects the detected lane markings onto the original video frames.

## 🔮 Future Scope

- Deep learning-based lane detection using CNN and LSTM architectures.
- Real-time traffic condition analysis.
- Integration with autonomous vehicle systems.
- Lane Departure Warning System (LDWS).
- Multi-lane detection and tracking.
- Improved performance under adverse weather conditions.

## 📚 References

1. Haris, M.; Hou, J. — *Obstacle Detection and Safe Navigation*, Sensors, 2020.
2. Yang, W.; Zhang, X.; Lei, Q. — *Lane Position Detection using LSTM*, Sensors, 2020.
3. Mammeri, A.; Boukerche, A.; Tang, Z. — *Real-Time Lane Localization*, 2015.
4. Sotelo, N.; Rodríguez, J.; Magdalena, L. — *Color Vision-Based Lane Tracking*, 2004.

## 📌 Conclusion

This project demonstrates a computer vision-based approach to road lane localization using Python and OpenCV. By combining image preprocessing, edge detection, perspective transformation, and Hough Transform, the system identifies lane markings and visualizes them on road video frames.

The project provides a foundation for further development in intelligent transportation systems, autonomous driving, and road safety applications.

---

## 👨‍💻 Author

**Selva Vishva M.**

B.Tech – Information Technology

GitHub: [@selvavishva](https://github.com/selvavishva)

---

⭐ If you find this project useful, consider giving it a star!
