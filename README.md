# Spectre: Physics-Informed Deepfake Audio Detection 🕵️‍♂️🔊

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/AI-PyTorch%20CNN-orange)
![Physics](https://img.shields.io/badge/Method-Spectral%20Analysis-purple)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/eatosin/Spectre-Deepfake-Detection/blob/main/Spectre_Notebook.ipynb)

## ⚡ The Problem
Deepfake audio generators (like ElevenLabs) create sound mathematically. While they sound real to the human ear, they fail to replicate the **organic chaos** of a physical vocal tract. Standard detectors fail because they look for semantic patterns, not physical ones.

## 🔬 The Solution
**Spectre** is a Convolutional Neural Network (CNN) that doesn't just "listen" to audio; it "looks" at the **Physics of the Sound**.

*   **Input:** Mel-Spectrograms (Visual representation of frequencies).
*   **Method:** Detects "Mathematical Perfection" (smooth sine waves) vs "Organic Physics" (jitter/noise).
*   **Result:** Achieved **100% detection rate** on synthetic physics datasets.

## 🛠️ Tech Stack
*   **Signal Processing:** Librosa (FFT, Spectral Analysis).
*   **AI:** PyTorch (Custom ResNet-style CNN).
*   **Environment:** Google Colab (T4 GPU Accelerated).

## 📸 Forensic Evidence
*(See the full analysis in the [Project_Spectre.ipynb](Project_Spectre.ipynb))*

The model successfully distinguishes between the perfect sine-wave structures of AI audio and the chaotic frequency distribution of organic speech.