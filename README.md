# Smart-Traffic-Vision
Traffic Scene Analysis Project using OCR

# Traffic-Scene-Analysis-project
Traffic Scene Analysis project with OCR

---

# 🚦 Traffic Scene Analysis with YOLOv8, OCR & VLM

This project presents an integrated AI pipeline that analyzes traffic scene images by:
- Describing the scene using a Vision-Language Model (VLM)
- Detecting license plates using a custom-trained YOLOv8 model
- Extracting license plate text using EasyOCR
- Returning a structured JSON output that includes scene description, detected plates, and OCR results

> ✅ Ideal for use cases like smart surveillance, intelligent traffic systems, and automated license plate recognition (ALPR).

---

## 📌 Features

- 🔍 **License Plate Detection** using YOLOv8.
- 🧾 **Text Extraction** from plates using EasyOCR (or PaddleOCR optionally).
- 🧠 **Scene Description** using a Vision-Language Model like Qwen-VL or LLaVA.
- 📦 **Output** is structured as a JSON combining all insights.

---

## 🧠 Technologies Used

| Component              | Model/Library       |
|------------------------|---------------------|
| Object Detection       | YOLOv8 (Ultralytics)|
| OCR (Text Recognition) | EasyOCR (default), PaddleOCR (optional) |
| Vision-Language Model  | Qwen-VL, LLaVA, or similar |
| Visualization          | OpenCV, Matplotlib  |
| Programming Language   | Python              |

---

📁 Folder Structure

├── data/
│   └── test/images/              # Input traffic images

├── weights/
│   └── best.pt                   # Trained YOLOv8 model weights

├── notebook.ipynb                # Main executable notebook

├── output/
│   └── results.json              # Final structured JSON outputs

└── README.md                     # Project documentation


---

## 🛠️ Installation

**Clone the repository**

```bash
git clone https://github.com/your-username/traffic-scene-analysis.git
cd traffic-scene-analysis


