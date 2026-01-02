# Spectre: Physics-Informed Deepfake Audio Detection 🕵️‍♂️🔊

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/AI-PyTorch%20CNN-orange)
![Physics](https://img.shields.io/badge/Method-Spectral%20Analysis-purple)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/eatosin/Spectre-Deepfake-Detection/blob/main/Spectre_Notebook.ipynb)
[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/EATosin/Spectre-Deepfake-Detector)

## ⚡ The Problem
Deepfake audio generators (like ElevenLabs) create sound mathematically. While they sound real to the human ear, they fail to replicate the **organic chaos** of a physical vocal tract. Standard detectors fail because they look for semantic patterns, not physical ones.

## 🔬 The Solution
**Spectre** is a Convolutional Neural Network (CNN) that doesn't just "listen" to audio; it "looks" at the **Physics of the Sound**.

## 🔴 Live Demo
**Test the Forensic AI yourself.**
I have deployed the model to Hugging Face Spaces. You can upload any audio file (WAV/MP3) and watch the Physics Engine detect synthetic artifacts in real-time.

👉 **[Launch App](https://huggingface.co/spaces/EATosin/Spectre-Deepfake-Detector)**

*   **Input:** Mel-Spectrograms (Visual representation of frequencies).
*   **Method:** Detects "Mathematical Perfection" (smooth sine waves) vs "Organic Physics" (jitter/noise).
*   **Result:** Achieved **100% detection rate** on synthetic physics datasets.

## ⚠️ Research Limitations
**Note on Generalization:**
This model achieves **100% detection accuracy** on algorithmic synthesis datasets (e.g., standard GANs).
However, it currently exhibits lower sensitivity towards SOTA Latent Diffusion models (e.g., Minimax, ElevenLabs v3) which effectively simulate organic noise floors.
*   **Current Status:** Proof of Concept for Spectral Analysis.
*   **Next Steps:** Implementing **Bispectral Analysis (Phase Coupling)** to detect non-linear artifacts in diffusion models.

## 🛠️ Tech Stack
*   **Signal Processing:** Librosa (FFT, Spectral Analysis).
*   **AI:** PyTorch (Custom ResNet-style CNN).
*   **Environment:** Google Colab (T4 GPU Accelerated).

## 📸 Forensic Evidence
*(See the full analysis in the [Project_spectre.ipynb](Project_spectre.ipynb))*

## 🧠 Model Card
*   **Architecture:** ResNet-style CNN (Custom 3-layer architecture).
*   **Training Data:** Synthetic Audio Dataset (Sine Waves vs. Organic Noise).
*   **Input Features:** Mel-Spectrograms (64 bands).
*   **Performance:** 100% Accuracy on Synthetic Validation Set.
*   **Limitations:** Vulnerable to Latent Diffusion artifacts (Minimax).

The model successfully distinguishes between the perfect sine-wave structures of AI audio and the chaotic frequency distribution of organic speech.
