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

## 💻 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/lung-sound-diagnosis.git
cd lung-sound-diagnosis
