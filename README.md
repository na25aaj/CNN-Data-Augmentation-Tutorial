# CNN Data Augmentation Tutorial: The Augmentation Experiment

### *How augmentation strategies affect generalisation: A controlled experiment on CIFAR-10*

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch 2.0+](https://img.shields.io/badge/PyTorch-2.0+-ee4c2c.svg)](https://pytorch.org/get-started/locally/)

---

## 📖 Overview
This repository contains a comprehensive machine learning tutorial exploring how different data augmentation strategies impact the generalisation of Convolutional Neural Networks (CNNs). Using the **CIFAR-10** dataset as a benchmark, we conduct a controlled experiment to measure how various transformations help close the "generalisation gap."

### The Six Strategies Compared:
| Strategy | Description |
| :--- | :--- |
| **Baseline** | No augmentation (Control condition) |
| **Flip + Crop** | Random horizontal flip + random padded crop |
| **Colour Jitter** | Random brightness, contrast, saturation, and hue |
| **Cutout** | Random rectangular region erased (Occlusion simulation) |
| **Combined** | Flip + Crop + Colour Jitter applied together |
| **Mixup** | Linear interpolation of image pairs and their labels |

---

## 📂 Repository Structure
```text
cnn-augmentation-tutorial/
├── notebook/
│   └── data_augmentation_tutorial.ipynb   # Main Jupyter notebook 
├── docs/
│   └── index.html                         # Tutorial web page (Results & Theory)
├── requirements.txt                       # Python dependencies
└── README.md                              # This file
