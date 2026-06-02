# TinyCNN: Ultra-Lightweight Heart Sound Classifier

[![Python](https://img.shields.io/badge/Python-3.12-blue.svg)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.10-red.svg)](https://pytorch.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

**TinyCNN** is an ultra-lightweight convolutional neural network for automated heart sound classification, specifically designed for **low-resource environments** such as rural healthcare centers, mobile devices, and edge-computing platforms.

With only **6,066 parameters** (15.4× smaller than a standard CNN, 1,842× smaller than ResNet18), TinyCNN achieves **72.72% ± 2.00% accuracy** and **0.8178 ROC-AUC** on 6,548 heart sound recordings, with **sub‑millisecond CPU inference**.

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

## 🗂️ Datasets

| Dataset | Samples | Normal | Abnormal | Use |
|---------|---------|--------|----------|-----|
| CirCor DigiScope | 3,007 | 2,391 | 616 | Training |
| PhysioNet/CinC 2016 | 3,541 | 2,725 | 816 | Training |
| **Combined** | **6,548** | **5,116 (78.1%)** | **1,432 (21.9%)** | **Training** |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/KSD301975/tinycnn-heart-sound.git
cd tinycnn-heart-sound
