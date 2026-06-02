markdown
# TinyCNN: Ultra-Lightweight Heart Sound Classifier

[![Python](https://img.shields.io/badge/Python-3.12-blue.svg)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0-red.svg)](https://pytorch.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📌 Overview

TinyCNN is an ultra‑lightweight convolutional neural network for automated heart sound classification, specifically designed for **low-resource environments** such as rural healthcare centers, mobile devices, and edge‑computing platforms.

With only **6,066 parameters** (15.4× smaller than a standard CNN, 1,842× smaller than ResNet18), TinyCNN achieves **72.72% ± 2.00% accuracy** and **0.8178 ROC-AUC** on 6,548 heart sound recordings, with **sub‑millisecond CPU inference** (1.002 ms/sample, 998 samples/second).

---

## 📊 Key Results

| Metric | Value |
|--------|-------|
| **Parameters** | **6,066** |
| **Accuracy** | **72.72% ± 2.00%** (3‑fold CV) |
| **ROC‑AUC** | **0.8178** |
| **CPU Inference** | **1.002 ms / sample** (998 samples/sec) |
| **GPU Memory** | **155 MB** |
| **Training Time** | **23 minutes** (NVIDIA T4) |

### Model Comparison

| Model | Accuracy | Parameters | Size vs TinyCNN |
|-------|----------|------------|-----------------|
| **TinyCNN (Ours)** | **72.72%** | **6,066** | **1×** |
| Baseline CNN | 74.53% | 93,378 | 15.4× |
| ResNet18 | 85.71% | 11,171,266 | 1,842× |

---

## 📁 Repository Structure
tinycnn-heart-sound/
├── tinycnn-heart-sound.ipynb # Complete training & evaluation notebook
├── figures/ # All manuscript figures (Fig. 1-7)
├── requirements.txt # Python dependencies
├── README.md # This file
└── (Pretrained weights will be added here)

text

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/KSD301975/tinycnn-heart-sound.git
cd tinycnn-heart-sound
