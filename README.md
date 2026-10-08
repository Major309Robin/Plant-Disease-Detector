# 🌿 Plant Disease Detector (By Robin John)

A deep learning project that detects plant type and disease from leaf images using PyTorch and a multi-task ResNet18 model, deployed with Streamlit. Designed as a portable, "plug-and-play" application running directly from a USB drive with zero configuration hassles and full protection against encoding issues and cache conflicts.

---

## 🚀 Project Features

* Classifies plant type 🌱
* Detects plant disease 🦠
* Built with PyTorch + ResNet18
* Web app using Streamlit
* Image preprocessing and augmentation
* **Portable USB Architecture:** Runs via an embedded Python environment (`python_embed`) without requiring prior installation on host computers.
* **Robust Execution:** Automated batch script automation (`Plant Disease Detector.exe`) to clear old cache files and enforce UTF-8 encoding.

---

## 🧠 Model Architecture

* Backbone: ResNet18 (pretrained)
* Feature extraction layer: 512 → 256
* Two output heads:
  * Plant classification head 🌱
  * Disease classification head 🦠

---

## 📂 Dataset

The dataset contains images of plant leaves categorized as:
* Apple, Tomato, Corn, Grape, etc.
* Each plant has different diseases + healthy class

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
├── Plant Disease Detector.bat
├── Plant Disease Detector.exe  # Plug & Play Launcher
└── README.txt
