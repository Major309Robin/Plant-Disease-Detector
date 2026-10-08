# 🌿 Plant Disease Detector (By Robin John)

A portable, "plug-and-play" Plant Disease Detection application built with PyTorch and Streamlit, designed to run directly from a USB drive with zero configuration hassles, completely protected against encoding issues (`UTF-8`) and cache conflicts.

## 🚀 Project Features

* **Plant Classification & Disease Detection:** Identifies plant types and detects leaf diseases accurately.
* **Portable USB Architecture:** Runs on an embedded Python environment (`python_embed`) without requiring Python installation on the host machine.
* **Web Interface:** Interactive and clean UI powered by Streamlit.
* **Robust & Clean Startup:** Automated cache cleanup and forced UTF-8 encoding via custom batch scripts (`run.bat`) to eliminate `Null Bytes` and environment errors.

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
├── python_embed/          # Embedded Python Environment (Portable)
├── scans_archive/
├── training/
│   └── train.py
├── Groq API Key.txt
├── planet_model.py
├── Plant Disease Detector.bat  # Main launcher script
└── README.md

 ## ⚙️ How to Run (Plug & Play)
Plug in your USB drive containing the project.

Double-click the Plant Disease Detector batch file (.bat).

The app will automatically clear old cache files, verify the embedded Python environment, and launch the Streamlit web app in your default browser at http://localhost:8501.

Developed with dedication by Robin John.
