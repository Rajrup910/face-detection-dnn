# Face Detection with Deep Learning (OpenCV DNN)

![Output](./docs/musk-output.jpg)

---

## 📌 Overview

This project implements **real-time face detection** using a deep learning model with OpenCV’s DNN module. It uses a pre-trained **Caffe-based SSD (Single Shot Detector)** model to detect faces in webcam streams or video files.

Compared to traditional methods like Haar Cascades, this approach provides **better accuracy and robustness** under different conditions.

---

## 🚀 Features

* Real-time face detection using webcam
* Deep learning-based detection (more accurate than traditional methods)
* Displays confidence score for each detected face
* Shows inference time for performance analysis
* Supports both webcam and video file input

---

## 📂 Project Structure

```
L1_05_Face_Detection_with_Deep_Learning/
│
├── Face_Detection_with_Caffe.py
├── models/
│   └── caffe/
│       ├── deploy.prototxt
│       └── res10_300x300_ssd_iter_140000_fp16.caffemodel
├── docs/
├── notebooks/
└── README.md
```

---

## ⚙️ Requirements

Install the required dependencies:

```
pip install opencv-python numpy
```

---

## ▶️ How to Run

### 🔹 Run using Webcam

```
python Face_Detection_with_Caffe.py
```

---

### 🔹 Run using Video File

```
python Face_Detection_with_Caffe.py video.mp4
```

---

## 🔁 How It Works

* Captures frames from webcam/video
* Converts image into a **blob format** using OpenCV
* Feeds blob into pre-trained deep learning model
* Model detects faces and outputs confidence scores
* Bounding boxes are drawn around detected faces
* Inference time is displayed on screen

---

## 🧪 Model Details

* Model: SSD (Single Shot Detector)
* Framework: Caffe
* Input Size: 300 × 300
* Confidence Threshold: 0.7

---

## 📸 Output

* Green bounding boxes around detected faces
* Confidence score displayed on each face
* Real-time inference time shown

---

## ⚠️ Notes

* Ensure model files are correctly placed inside `models/caffe/`
* Press **ESC key** to exit the application
* Works best in good lighting conditions

---

## 📚 Future Improvements

* Add face recognition (identify person)
* Improve performance using GPU
* Add emotion detection
* Convert into a web-based application

---

## 🤝 Contributing

Contributions are welcome! You can:

* Add new models or improvements
* Optimize performance
* Fix bugs or enhance features

Steps:

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Push and create a pull request

---

## 📖 References

* https://github.com/opencv/opencv/tree/4.x/samples/dnn

---

## 👨‍💻 Author

Developed as part of a computer vision learning project.
