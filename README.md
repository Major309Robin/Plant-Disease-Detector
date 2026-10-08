# 🌿 Plant Disease Detection using Deep Learning

A deep learning project that detects plant type and disease from leaf images using PyTorch and a multi-task ResNet18 model, deployed with Streamlit. Designed as a portable, "plug-and-play" application running directly from a USB drive with zero configuration hassles and full protection against encoding issues and cache conflicts.

---

## 🚀 Project Features

* Classifies plant type 🌱[cite: 13]
* Detects plant disease 🦠[cite: 13]
* Built with PyTorch + ResNet18[cite: 13]
* Web app using Streamlit[cite: 13]
* Image preprocessing and augmentation[cite: 13]
* **Portable USB Architecture:** Runs via an embedded Python environment (`python_embed`) without requiring prior installation on host computers.
* **Robust Execution:** Automated batch script automation (`run.bat`) to clear old cache files and enforce UTF-8 encoding.

---

## 🧠 Model Architecture

* Backbone: ResNet18 (pretrained)[cite: 13]
* Feature extraction layer: 512 → 256[cite: 13]
* Two output heads:[cite: 13]
  * Plant classification head 🌱[cite: 13]
  * Disease classification head 🦠[cite: 13]

---

## 📂 Dataset

The dataset contains images of plant leaves categorized as:[cite: 13]
* Apple, Tomato, Corn, Grape, etc.[cite: 13]
* Each plant has different diseases + healthy class[cite: 13]

---

## 📁 Project Structure

```text
Plant-Disease-Detector/
│
├── app/
│   └── planet_app.py
├── Database/
├── model/
│   ├── planet_model.py
│   └── model.pth
├── python_embed/          # Embedded Portable Python
├── scans_archive/
├── training/
│   └── train.py
├── Groq API Key.txt
├── Plant Disease Detector.bat  # Plug & Play Launcher
└── README.md
