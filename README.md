# 🚗 Number Plate Detection System using YOLOv8 & Flask

## 📌 Overview

This project is a web-based Vehicle Number Plate Detection System developed using **YOLOv8**, **Flask**, and **OpenCV**. Users can upload an image containing a vehicle, and the application automatically detects and highlights the number plate using a custom-trained YOLO model.

---

## ✨ Features

* Upload images through a web interface
* Detect vehicle number plates using a trained YOLOv8 model
* Draw bounding boxes around detected plates
* Display processed images instantly
* Lightweight Flask web application
* Easy deployment and customization

---

## 🛠 Technologies Used

* Python 3.x
* Flask
* YOLOv8 (Ultralytics)
* OpenCV
* HTML5
* CSS3

---

## 📂 Project Structure

```
NumberPlateDetection/
│
├── app.py
├── best.pt
├── requirements.txt
├── README.md
│
├── templates/
│   └── index.html
│
├── static/
│   ├── uploads/
│   └── results/
│
└── screenshots/
    ├── input.png
    └── output.png
```

---

## ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/number-plate-detection.git
cd number-plate-detection
```

### Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

**Windows**

```bash
venv\Scripts\activate
```

**Linux/Mac**

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install flask ultralytics opencv-python
```

or

```bash
pip install -r requirements.txt
```

---

## 📥 Model File

Place your trained YOLO model file (`best.pt`) in the project root directory.

```
NumberPlateDetection/
│
├── app.py
├── best.pt
```

---

## ▶️ Running the Application

Start the Flask server:

```bash
python app.py
```

The application will run at:

```text
http://127.0.0.1:5000
```

Open the URL in your browser.

---

## 🔄 Workflow

1. User uploads a vehicle image.
2. Flask saves the uploaded image.
3. YOLOv8 processes the image.
4. Number plate is detected.
5. Bounding boxes are drawn.
6. Result image is saved.
7. Output is displayed on the webpage.

---

## 🧠 Model Information

* Model: YOLOv8 Custom Model
* Task: Number Plate Detection
* Framework: Ultralytics YOLO
* Output: Bounding Box Coordinates and Confidence Score

---

## 📸 Supported Image Formats

* JPG
* JPEG
* PNG
* BMP

---

## 📷 Sample Output

### Input

Vehicle image uploaded by the user.

### Output

Vehicle image with detected number plate highlighted using a bounding box.

---

## 🚀 Future Enhancements

* OCR for reading plate numbers
* Real-time webcam detection
* Video processing support
* Vehicle tracking
* Database integration
* Export results as PDF/CSV

---

## 🐞 Common Issues

### Model Not Found

Error:

```text
FileNotFoundError: best.pt
```

Solution:

Ensure that `best.pt` is located in the project root folder.

### Flask Module Missing

```bash
pip install flask
```

### OpenCV Module Missing

```bash
pip install opencv-python
```

---
