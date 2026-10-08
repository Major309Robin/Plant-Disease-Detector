
# 🌿 Plant Disease Detection using Deep Learning

A deep learning project that detects plant type and disease from leaf images using PyTorch and a multi-task ResNet18 model, deployed with Streamlit.

---

## 🚀 Project Features
- Classifies plant type 🌱  
- Detects plant disease 🦠  
- Built with PyTorch + ResNet18  
- Web app using Streamlit  
- Image preprocessing and augmentation  

---

## 🧠 Model Architecture
- Backbone: ResNet18 (pretrained)
- Feature extraction layer: 512 → 256
- Two output heads:
  - Plant classification head 🌱
  - Disease classification head 🦠

---

## 📂 Dataset
The dataset contains images of plant leaves categorized as:

- Apple, Tomato, Corn, Grape, etc.
- Each plant has different diseases + healthy class

---

## 📁 Project Structure

```
plant-disease-detection/
│
├── app/
│   └── planet_app.py
│
├── model/
│   ├── planet_model.py
│   └── model.pth
│
├── training/
│   └── train.py
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 📥 How to Download & Install
Go to the repository Releases section on GitHub.

Download the ready-to-use portable package Plant.Disease.Detector.zip from the latest release assets.

Extract the ZIP file directly onto your USB flash drive or local machine.

---

## ⚙️ How to Run
Plug in your USB drive or open the extracted project folder.

Double-click the application launcher (Plant Disease Detector.exe or the batch file).

The app will automatically clear old cache, verify the embedded Python environment, and launch the Streamlit web app in your default browser at http://localhost:8501.

---

## Developed with dedication by Robin John.
---
