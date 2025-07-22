# 🗣️ Arabic /r/ Sound Pronunciation Disorder Detection

This project applies machine learning techniques to classify pronunciation disorders in the Arabic /r/ phoneme. Developed for the **Spoken Language Processing** course (Spring 2024/2025), the goal is to automatically detect whether the /r/ sound at the beginning of a word is correctly pronounced or misarticulated.

---

## 📘 Project Description

Arabic-speaking children often struggle with the /r/ phoneme, leading to various speech disorders. This project focuses on identifying five pronunciation categories:

1. ✅ Normal pronunciation  
2. 🔁 Distortion    
3. 🔄 Substitution with /gh/  
4. 🔃 Substitution with /l/  

We built a complete classification system using audio features and several machine learning models.

---

## 🧪 Dataset

- Audio recordings (WAV files)
- Pre-labeled into 5 folders (one per class)
- Split into `Train` and `Test` directories
- Source: Provided by course instructors

---

## 🎯 Features

- **MFCCs (Mel-Frequency Cepstral Coefficients)**
- Delta and Delta-Delta derivatives
- Fixed-length feature vectors
- PCA used for dimensionality reduction (for GMM)

---

## 🤖 Models Evaluated

| Model                  | Accuracy |
|------------------------|----------|
| Random Forest          | 75.00%   |
| SVM (RBF kernel)       | 70.25%   |
| Gaussian Mixture Model | 57.50%   |
| HistGradientBoosting   | **75.25%** 🔥 |
| Stacking Ensemble      | 74.75%   |
| Voting Ensemble        | 72.75%   |

> ✅ **Best model**: `HistGradientBoostingClassifier`  
> 📊 Evaluation metrics: Accuracy, Precision, Recall, F1-score


