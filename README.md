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

## 🎥 Demo Video

https://github.com/user-attachments/assets/9f1c751f-0d08-4a92-9610-a52a5f74f1c9

---

🖼️ Sample Output

<img width="1911" height="859" alt="Screenshot (488)" src="https://github.com/user-attachments/assets/0a1d309b-2ce2-4a7b-b258-6a960f7c53b4" />
<img width="1920" height="859" alt="Screenshot (489)" src="https://github.com/user-attachments/assets/db1ec644-aba2-401a-9ddb-b2ddc0be60c7" />

---

## 📌 Features

- 🔍 **License Plate Detection** using YOLOv8.
- 🧾 **Text Extraction** from plates using EasyOCR (or PaddleOCR optionally).
- 🧠 **Scene Description** using a Vision-Language Model like Qwen-VL or LLaVA.
- 📦 **Output** is structured as a JSON combining all insights.

---
## 📁 Project Folder Structure

Smart-Traffic-Vision/
├── README.md                       # Project documentation

├── yolo11n.pt                      # Custom-trained YOLOv8 model

├── yolov8n.pt                      # Pretrained YOLOv8 model

├── data (1).yaml                   # YOLO dataset config

│

├── data/                           # data (Train ,test and valid)

│

├── notebooks/                      # Jupyter notebooks for testing and development

│   └── *.ipynb

│

├── images for test/               # Images used for testing the pipeline

│   ├── image1.jpg

│   └── image2.jpg

│

├── runs/                           # YOLO training runs (Ultralytics output)

│   └── detect/

│       └── train/

│           ├── weights/

│           │   └── best.pt

│           └── ...

│

├── runs_backup/                    # Backup of training runs

│   └── detect/

│       └── train/

│           └── ...

│

├── sample output of json/          # Example structured JSON results

│   └── output1.json

│

├── Screenshot and vedio/           # Demo assets

│   ├── demo_video.mp4

│   └── screenshot1.png


---

## 🧠 Technologies Used

| Component              | Model/Library       |
|------------------------|---------------------|
| Object Detection       | YOLOv8 (Ultralytics)|
| OCR (Text Recognition) | EasyOCR , PaddleOCR  |
| Vision-Language Model  | Qwen-VL, LLaVA, blip2-opt-2.7b or similar |
| Visualization          | OpenCV, Matplotlib  |
| Programming Language   | Python              |

---

## 🚀 Usage
Prepare input images

Place your traffic scene images inside the data/test/images/ folder.

Run the notebook

Open and run notebook.ipynb in Kaggle, Google Colab, or your local Jupyter environment.

Pipeline Stages

🔧 Load YOLOv8 model and OCR engine

🖼️ Read and visualize a sample of 15 images

🏷️ Detect license plates in each image

🔡 Run OCR to extract license plate text

📜 Use a VLM to generate a scene caption

🧾 Output a consolidated JSON report


---

## 🎯 Applications
🚗 Smart Traffic Monitoring

🛑 Automated Violation Detection

🏙️ Urban Surveillance Systems

🚓 Law Enforcement Tools

---

## 📈 Future Improvements
Integrate real-time video stream input.

Add support for multilingual OCR.

Improve plate formatting and post-processing.

Integrate map or GPS metadata for tracking.

---

## 👤 Author
Developed by Israa Mohamed Gaber
🔗 LinkedIn: https://www.linkedin.com/in/israamohamedgaber/
📧 Email: mohamedisraa23@gmail.com
