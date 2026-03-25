CNN Data Augmentation Tutorial
How augmentation strategies affect generalisation: A controlled experiment on CIFAR-10
License: MIT Python 3.8+ PyTorch

Overview
This repository contains all materials for a machine learning tutorial exploring how different data augmentation strategies affect CNN generalisation on the CIFAR-10 image classification benchmark.

Six strategies are compared in a controlled experiment:

Strategy	Description
Baseline	No augmentation
Flip + Crop	Random horizontal flip + random crop
Colour Jitter	Random brightness, contrast, saturation, hue
Cutout	Random rectangular region erased
Combined	Flip + Crop + Colour Jitter together
Mixup	Linear interpolation of image pairs and their labels
Repository Structure

cnn-augmentation-tutorial/
├── notebook/
│   └── data_augmentation_tutorial.ipynb   # Main Jupyter notebook 
├── docs/
│   └── index.html                         # Tutorial web page
├── requirements.txt                       # Python dependencies
└── README.md                              # This file

Requirements
See requirements.txt. Key dependencies:

Python 3.8+
PyTorch >= 2.0
torchvision >= 0.15
matplotlib >= 3.6
seaborn >= 0.12
numpy >= 1.23
tqdm >= 4.64
jupyter >= 1.0
Reproducing Results
All experiments use SEED = 42 for reproducibility. The notebook is designed to be run top to bottom without modification. GPU is detected automatically; CPU is supported.

Expected training time: ~3–5 minutes on a modern GPU, ~10–15 minutes on CPU (30 epochs × 6 experiments).

Accessibility
The tutorial web page (docs/index.html) is designed with accessibility in mind: - Colourblind-safe palette (Wong, 2011, Nature Methods) - Semantic HTML with ARIA labels - Skip navigation link - Sufficient colour contrast (WCAG AA compliant) - All figures include descriptive alt-text / ARIA labels

References
Krizhevsky, A. (2009). Learning Multiple Layers of Features from Tiny Images. Technical Report, University of Toronto.
DeVries, T., & Taylor, G. W. (2017). Improved Regularization of Convolutional Neural Networks with Cutout. arXiv:1708.04552.
Zhang, H., Cisse, M., Dauphin, Y. N., & Lopez-Paz, D. (2018). Mixup: Beyond Empirical Risk Minimization. ICLR 2018.
Shorten, C., & Khoshgoftaar, T. M. (2019). A survey on image data augmentation for deep learning. Journal of Big Data, 6(1), 1–48.
Wong, B. (2011). Points of view: Color blindness. Nature Methods, 8(6), 441.
Licence
This project is released under the MIT Licence. You are free to use, modify, and distribute this work with attribution.
