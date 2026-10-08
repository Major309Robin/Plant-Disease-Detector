# 🌿 Plant Disease Detection & Smart Diagnosis System

A comprehensive deep learning and AI-powered project that detects plant types and diseases from leaf images using PyTorch and a multi-task ResNet18 model, deployed interactively with Streamlit. Featuring multi-language support, real-time weather & seasonal guides, SQLite scan archiving, and an AI Plant Doctor assistant.

---

## 🚀 Key Features & Capabilities

* **Dual-Task Deep Learning Detection:** Accurately classifies plant species and detects specific diseases simultaneously using a custom ResNet18 backbone.
* **Bilingual Interface (English & العربية):** Full support for English and Arabic languages with seamless layout and text adaptation.
* **Smart Weather & Season Inspector:** Integrates live location/weather tracking via `wttr.in` and automated seasonal analysis to verify if the plant matches the current season.
* **Plant Doctor AI Assistant (Groq API):** Interactive chatbot powered by Groq API (`openai/gpt-oss-20b`) that gives expert agricultural advice tailored to the scanned plant, weather, and diagnosis.
* **SQLite Database & Archiving:** Automatically saves scans, high-resolution images (`scans_archive`), detailed text reports, and chat histories into a local SQLite database (`Database/plant_scans.db`).
* **Analytics & Search Dashboard:** Filter past scans by status (Healthy/Diseased), search records by plant or disease name, export history as a CSV file for Excel, and view quick analytics/recent scans.
* **Custom UI & Dark Mode:** Toggle between Dark and Light themes with custom CSS styling, upload helper guides, and report download/copy features[cite: 1].

---

## 🧠 Model Architecture

* **Backbone:** Pretrained ResNet18 model (with final classification layer adapted)[cite: 1].
* **Feature Extraction Layer:** Fully connected layer mapping 512 features to 256 units[cite: 1].
* **Dual Output Heads:**
  * **Plant Classification Head 🌱** (handles 14 plant types)[cite: 1]
  * **Disease Classification Head 🦠** (handles 21 disease/health classes)[cite: 1]

---

## 📂 Supported Categories

* **Plants (14 types):** Apple, Blueberry, Cherry (including sour), Corn (maize), Grape, Orange, Peach, Pepper (bell), Potato, Raspberry, Soybean, Squash, Strawberry, and Tomato[cite: 1].
* **Conditions & Diseases (21 classes):** Includes various blights, spots, rusts, mildews, viruses, and healthy classifications[cite: 1].

---

## 📁 Project Structure

```text
plant-disease-detection/
│
├── app/
│   └── planet_app.py        # Streamlit web application & UI
│
├── model/
│   ├── planet_model.py      # Model architecture definition
│   └── model.pth            # Trained weights file
│
├── Database/                # SQLite database folder (auto-created)
│   └── plant_scans.db
│
├── scans_archive/           # Saved scan images folder (auto-created)
│
├── training/
│   └── train.py             # Model training script
│
├── Groq API Key.txt         # Saved Groq API key storage
├── requirements.txt
├── .gitignore
└── README.md
```
---

## 📥 Download & Install

1. Go to the repository Releases section on GitHub.
2. Download the portable package Plant.Disease.Detector.zip.
3. Extract the ZIP file onto your computer or USB drive.

---

## ⚙️ How to Run
1. Open the extracted project folder.

2. Double-click the application launcher (Plant Disease Detector.exe or batch file).

3. The app will launch automatically in your browser.

---

Developed with dedication by Robin John
