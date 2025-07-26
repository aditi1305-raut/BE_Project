# Diagnosing Respiratory Conditions via Lung Sound using CNN and LSTM

A deep learning-based system that diagnoses respiratory diseases using lung sound recordings. This project combines Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) models to automatically classify lung sounds like wheezes, crackles, and rhonchi to aid in early detection of conditions such as asthma, pneumonia, bronchitis, and COPD.

---

## 🧠 Abstract

This project presents a cost-effective, non-invasive, and accurate system for diagnosing respiratory conditions using machine learning. We extract Gammatone Cepstral Coefficients (GTCC) and Short-Time Fourier Coefficients (STFC) features from lung sounds and classify them using CNN-LSTM models. The system processes over 6800 audio clips, achieving a peak accuracy of **99.22%**.

---

## 📌 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [System Architecture](#-system-architecture)
- [Installation](#-installation)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Testing](#-testing)
- [Results](#-results)
- [Limitations](#-limitations)
- [Contributors](#-contributors)
- [License](#-license)

---

## ✅ Features

- Upload lung audio recordings.
- Automatic preprocessing and feature extraction (GTCC, MFCC).
- CNN for spatial analysis, LSTM for temporal analysis.
- Classify lung sounds as: Healthy, Crackles, Wheezes, Rhonchi.
- Admin interface for managing users and monitoring system use.
- Responsive web application built with HTML/CSS/JS.

---

## 🛠 Tech Stack

**Frontend**
- HTML
- CSS
- JavaScript

**Backend**
- Python 3.8
- Flask

**Libraries**
- TensorFlow / Keras
- Librosa
- NumPy, Pandas
- Matplotlib / Seaborn

**Tools**
- Visual Studio Code
- Anaconda Navigator

---

## 🏗️ System Architecture

1. **Input**: Lung sound recording (`.wav` or `.mp3`)
2. **Preprocessing**: Noise filtering, feature extraction (MFCC/GTCC)
3. **Model**: CNN layers + LSTM layers
4. **Prediction**: Classify audio into respiratory condition
5. **Output**: Display result with probability score

---

lung-sound-diagnosis/
│
├── app.py                  # Main Flask app
├── models/                 # Trained CNN-LSTM models
├── data/                   # Dataset (e.g., ICBHI 2017)
├── static/                 # CSS/JS files
├── templates/              # HTML templates
├── preprocessing.py        # Audio preprocessing pipeline
├── classify.py             # Classification logic
├── requirements.txt        # Python dependencies
├── README.md               # Project overview
└── report/                 # Project report and documentation

🚀 Usage
-Open the app in a browser at http://127.0.0.1:5000.

-Upload a .wav file of lung sound.

-Get a diagnosis (e.g., Healthy, Crackles, Wheezes, etc.).

-View confidence score and suggested preventive measures.

🧪 Testing
Types of Testing Performed:
-Unit Testing: Feature extraction, segmentation, model prediction

-Integration Testing: Audio pipeline through UI to model

-Functional Testing: User login, file upload, prediction output

-System Testing: Full-stack test from frontend to model output

-Cross-validation: 5-fold CV on dataset

-Performance Metrics:

  -Accuracy: 99.22%

  -AUC: 0.93

Precision: High across all classes

📊 Results
1.Highest accuracy: 99.22%

2.Evaluated on 6800+ audio clips

3.CNN-LSTM outperformed baseline MLP models

4.Real-time processing within 1-2 seconds per clip

⚠️ Limitations
1.Requires Internet connection to function fully (for updates or deployment).

2.Limited performance in very noisy environments or low-quality audio.

3.Requires a dataset with labeled lung sounds for retraining.

👨‍💻 Contributors
1.Rohit Pawar

2.Aditi Raut

3.Sneha Jadhav

Under the guidance of: Prof. Shah S. N.

📃 License
This project is licensed under the MIT License - see the LICENSE file for details.

📚 References
1.ICBHI 2017 Challenge Dataset

2.Librosa Documentation

3.TensorFlow/Keras Docs

4.CNN

5.LSTM

📌 Acknowledgment
This work was completed as part of the Bachelor of Engineering (Computer Engineering) curriculum at SSPM's Sharadchandra Pawar College of Engineering and Technology, affiliated with Savitribai Phule Pune University, 2024–2025.

