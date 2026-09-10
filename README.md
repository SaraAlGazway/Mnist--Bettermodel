# 🧠 MNIST BetterModel Classifier with PyTorch

An improved neural network for handwritten digit recognition 
using PyTorch and the MNIST dataset.

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0-red)
![License](https://img.shields.io/badge/License-MIT-green)

## 🎯 Results

| Metric | Value |
|--------|-------|
| Test Accuracy | **97.69%** |
| Final Train Accuracy | 98.34% |
| Total Parameters | 101,770 |
| Training Epochs | 10 |

## 📚 What This Notebook Covers

- ✅ Loading MNIST dataset
- ✅ Building a Better Neural Network (Hidden Layer + ReLU + Dropout)
- ✅ Training the model for 10 epochs
- ✅ Evaluating on test set
- ✅ Visualizing predictions

## 🏗️ Model Architecture

| Layer | Type | Input | Output |
|-------|------|-------|--------|
| 1 | Flatten | (1, 28, 28) | 784 |
| 2 | Linear | 784 | 128 |
| 3 | ReLU | 128 | 128 |
| 4 | Dropout (0.2) | 128 | 128 |
| 5 | Linear | 128 | 10 |

**Total Parameters**: 101,770

## ⚙️ Training Configuration

| Hyperparameter | Value |
|----------------|-------|
| Batch Size | 64 |
| Learning Rate | 0.001 |
| Optimizer | Adam |
| Loss Function | CrossEntropyLoss |

## 📊 Training Progress

| Epoch | Loss | Accuracy |
|-------|------|----------|
| 1 | 0.3739 | 89.73% |
| 5 | 0.0894 | 97.26% |
| 10 | 0.0515 | **98.34%** |

## 🛠️ Technologies Used

- Python 3.10
- PyTorch 2.0
- Torchvision
- Matplotlib
- NumPy

## 🚀 How to Run

### On Kaggle
1. Open the notebook on Kaggle
2. Enable GPU (Settings → Accelerator → GPU)
3. Run all cells

### Locally
```bash
pip install -r requirements.txt
jupyter notebook mnist-bettermodel.ipynb
