# 🐦 Bird Species Classification Based on Audio Using Deep Learning (MFCC & Mel-Spectrogram)

This repository contains the implementation of a deep learning-based approach to classify **six bird species** from their audio recordings using two powerful audio features: **Mel-Spectrogram** and **Mel-Frequency Cepstral Coefficients (MFCC)**.

## 📌 Research Objective

To develop a robust classification system that can automatically identify bird species based on audio signals, using deep learning models such as **Convolutional Neural Networks (CNN)**, **MobileNet**, and **VGGish architectures** trained on Mel-Spectrogram and MFCC representations.

## 🐤 Bird Species Included

- Cendet (Lanius schach)
- Burung Gereja (Passer domesticus)
- Kutilang (Pycnonotus aurigaster)
- Perkutut (Geopelia striata)
- Tekukur (Streptopelia chinensis)
- Trucukan (Pycnonotus goiavier)

## 🧠 Methodology Overview

1. **Preprocessing**:
   - Pre-emphasis
   - Framing (25 ms frame size, 10 ms stride)
   - Windowing (Hamming)
   - Short-Time Fourier Transform (STFT)

2. **Feature Extraction**:
   - **Mel-Spectrogram** (128 filters)
   - **MFCC** (40 coefficients)

3. **Classification**:
   - CNN , MobileNet, and VGGish models
   - Trained using Categorical Cross Entropy and Adam optimizer

4. **Evaluation Metrics**:
   - Accuracy
   - Confusion Matrix
   - Precision, Recall, F1-Score per class

## 📈 Results Summary

- **Best Model**: CNN with MFCC input
- **Accuracy Test**: 97.97%
- **Precision (avg) Test**: 97.78%
- **Recall (avg)**: 98.27%
- **F1-Score (avg)**: 97.96%

## 📂 Project Structure

```bash
├── data/
│   ├── audio/              # Raw and trimmed bird sound files
│   ├── spectrogram/        # Mel-Spectrogram images
│   ├── mfcc/               # MFCC features
│
├── models/
│   ├── cnn_model.h5        # Trained CNN model
│   └── vgg_model.h5        # Trained VGG model
│
├── notebooks/
│   ├── preprocessing.ipynb # Preprocessing and feature extraction
│   ├── training.ipynb      # Model training and evaluation
│
├── Paper.pdf               # Final paper (in Bahasa Indonesia)
└── README.md               # Project description

```
## 🔗 Citation

If you use this code or data in your research, please cite:

> Putra, D. (2025). *Klasifikasi Spesies Burung Berdasarkan Suara Burung Menggunakan Deep Learning dengan Fitur Mel-Spektogram dan MFCC*. Surabaya: Institut Teknologi Sepuluh Nopember.

## 📬 Contact

For more information or collaboration:

**Daniswara Putra**  
📧 **Email**: daniswara.dap@gmail.com  
🐙 **LinkedIn:** [linkedin.com/in/daniswara-aditya-putra](https://www.linkedin.com/in/daniswara-aditya-putra)

---

✨ Made with deep learning and birdsong!

