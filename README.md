## A Comprehensive Comparative Study on Speech Emotion Recognition using Multi-Dataset, Multi-Feature, and Multi-Model Approaches 

<div align="center">
  <img src="https://img.shields.io/badge/Language-Python-blue?style=for-the-badge&logo=python" />
  <img src="https://img.shields.io/badge/Framework-PyTorch-red?style=for-the-badge&logo=pytorch" />
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/Audio%20Features-Librosa-yellow?style=for-the-badge&logo=librosa" />
</div>

---

### 📘 Project Overview

This project conducts a detailed multi-dataset, multi-model, and multi-feature comparative study in the domain of Speech Emotion Recognition (SER). It evaluates the effectiveness of both classical machine learning algorithms and deep learning models on the RAVDESS and SAVEE datasets, using a range of acoustic feature sets including MFCC-13, MFCC-40, delta and delta-delta coefficients, ZCR, RMS, and OpenSMILE descriptors.

---

### 🧠 Objectives

- Compare classical machine learning models and deep learning architectures for Speech Emotion Recognition.
- Investigate the effectiveness of various acoustic feature sets, including MFCC-13, MFCC-40, MFCC with delta & delta-delta (MFCC-39), and MFCC-40 combined with ZCR and RMS.
- Evaluate model performance across diverse multi-speaker datasets, specifically RAVDESS and SAVEE.
- Assess the influence of dataset size and feature richness on model accuracy and generalization capability.

---

### 🧰 Tech Stack & Tools

| Domain | Tools & Libraries |
|-------|--------------------|
| **Languages** | <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" /> |
| **ML Models** | <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" /> |
| **DL Models** | <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" /> |
| **Audio Processing** | <img src="https://img.shields.io/badge/Librosa-903BAE?style=flat-square" />, <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" /> |
| **Visualization** | <img src="https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=matplotlib&logoColor=white" />, <img src="https://img.shields.io/badge/Seaborn-7E7F9A?style=flat-square" /> |

---

### 🧪 Datasets Used

#### 🎤 RAVDESS
- 24 actors (12 male, 12 female)
- 8 emotions
- Studio-quality recordings
- Balanced gender representation

#### 🧑 SAVEE
- 4 male speakers
- 7 emotions
- British accent

---

### 🔍 Feature Extraction

We used **Librosa** for all audio processing and feature extraction, along with **OpenSMILE** for advanced feature descriptors. The following feature sets were extracted and evaluated independently across all models:

- 🎵 **MFCC-13**  
  Standard 13 Mel-Frequency Cepstral Coefficients capturing short-term power spectrum.

- 🔄 **MFCC-39 (MFCC + Δ + ΔΔ)**  
  Includes first and second-order derivatives to capture temporal dynamics.

- 🧠 **MFCC-40 + ZCR + RMS**  
  Extended feature set combining 40 MFCCs with:
  - **ZCR** (Zero-Crossing Rate) – a prosodic feature  
  - **RMS** (Root Mean Square Energy) – a spectral feature  

- 🔬 **OpenSMILE Feature Set**  
  Extracted using the **INTERSPEECH 2010 Paralinguistic Challenge configuration**, this set includes:
  - Energy-based features (e.g., loudness, RMS energy)  
  - Voicing features (e.g., jitter, shimmer, HNR)  
  - Spectral features (e.g., centroid, flux, roll-off)  
  - Prosodic and pitch-based features  

These diverse feature sets enabled a thorough performance comparison across models and datasets.

---

### 🤖 Models Implemented

| Model Type | Algorithms |
|------------|------------|
| **Machine Learning** | SVM, XGBoost|
| **Deep Learning** | DCNN, LSTM |

Each model was evaluated with multiple feature sets. Starting with MFCC 13, MFCC DD, MFCC 40, MFCC40+ZCR+RMS, OpenSmile

---

### 📊 Evaluation Metrics

- 🎯 Accuracy
- 📉 Loss
- 📈 F1-Score
- Confusion matrix

Each metric was logged during training and testing for comparative insights.

---

### 📌 Key Highlights

- 🔬 **40 Dimensional MFCC 40 Feature set** yielded high accuracy in most cases.
- 💡 **XgBoost achieved good accuracy in smaller dataset while SVM achieved good accruacy in comparatively bigger dataset** achieved the best performance in machine learning.
- 💡 **DCNN achieved good accuracy than LSTM** and was the best performing model in deep learning.
- ⚖️ Dataset size, diversity and balance played a critical role in generalization.

---

### 📎 Results
See the full results in the provided excel document CompAnalysis.xlsx

---

### 💬 Contact

For questions or collaborations:  
📧 preetam_teja@outlook.com

---
