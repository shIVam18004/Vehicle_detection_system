# 🚗 Vehicle Counter Detection

A computer vision-based Python project to automatically detect and count vehicles in a video stream using OpenCV. This tool visually tracks vehicles crossing a virtual line, useful for traffic analysis or surveillance applications.

---

## 🚀 Live Preview

🖥️ **Not applicable** – This is a desktop-based Python script.  
▶️ Just run the `vehicle.py` script locally on your machine with a video file.

---

## 📸 Screenshots

📷 Vehicle Detection and Counting Screenshot  
_Add your screenshot as `screenshot.png` in the root directory._
![Alt text 1](https://github.com/shIVam18004/Vehicle_detection_system/blob/main/vehicle_1.png)
![Alt text 2](https://github.com/shIVam18004/Vehicle_detection_system/blob/main/vehicle_2.png
)

---

## 🛠️ Features

✅ Detect moving vehicles using background subtraction  
🚦 Count vehicles crossing a virtual line  
📷 Real-time bounding box and center-point drawing  
🧠 Simple logic using contours and object tracking  
📊 Live counter displayed on each video frame  
📁 Minimal dependencies and setup  

---

## 🧩 Elements and Structure

### 📁 Folder Structure
```
Vehicle-Counter-Detection/
│
├── myenv/                # Python virtual environment
│
├── vehicle.py            # Main script for detection and counting
├── video.mp4             # Input video (not included in repo)
└── screenshot.png        # Output image sample (add this manually)
```

---

### 🖥️ Technologies Used

- **Python 3**
- **OpenCV** – Image processing, contour detection, video I/O
- **NumPy** – For array operations

---

## 🔍 Core Logic

### 🎥 Frame Processing

- Convert each frame to grayscale
- Apply Gaussian blur for noise reduction
- Use `cv2.createBackgroundSubtractorMOG2()` for motion segmentation

### 🔎 Object Detection

- Detect contours from the processed frames
- Filter out noise by minimum width and height
- Draw bounding boxes and compute object centers

### 📈 Vehicle Counting

- Track when the object center crosses a horizontal count line
- Maintain a counter and remove already-counted vehicles

---

## 🧠 What I Learned

💡 Motion-based detection using background subtraction  
💡 Real-time video analysis using OpenCV  
💡 Drawing and overlaying text and shapes in frames  
💡 Filtering and tracking techniques for dynamic scenes  

---

## 📂 Tech Stack

- **Python 3**
- **OpenCV**
- **NumPy**

---

## 🧪 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/shIVam18004/Vehicle_detection_system.git
   cd Vehicle_detection_system
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv myenv
   myenv\Scripts\activate     # For Windows
   source myenv/bin/activate # For Linux/Mac
   ```

3. Install dependencies:
   ```bash
   pip install opencv-python numpy
   ```

4. Add a video file named `video.mp4` to the root directory.

5. Run the script:
   ```bash
   python vehicle.py
   ```

---

## ⚠️ Deployment Notes

🚫 Not suitable for deployment in cloud/web environments (e.g., Streamlit, Flask) due to:
- Dependency on local video input and OpenCV GUI window
- No REST API or web interface
- Designed for local execution only

---

## 📈 Future Enhancements

- Replace background subtraction with YOLO or deep learning models  
- Classify vehicle types (car, truck, bike)  
- Build a web dashboard using Flask/Streamlit  
- Log counts to a file or database  

---

## 📁 Resources

📄 [ReadMe](README.md)  
💻 [Project Activity](https://github.com/shIVam18004)  
⭐ Stars: 0 | 👀 Watchers: 1 | 🍴 Forks: 0  
