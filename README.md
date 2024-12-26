# MT

This repository contains the code and resources for a brain tumor classification project using deep learning. The study explores the impact of data augmentation and explainable AI (XAI) techniques, such as LIME, SHAP, and Grad-CAM, to improve performance and interpretability.

## Features
- **Multi-class Brain Tumor Classification:** Glioma, Meningioma, Pituitary Tumor, and No Tumor.
  - REF: Msoud Nickparvar. (2021). Brain Tumor MRI Dataset [Data set]. Kaggle. https://doi.org/10.34740/KAGGLE/DSV/2645886
- **Data Augmentation:** 
  - Traditional (e.g., TrivialAugment)
  - Generative (GAN-based synthetic data)
  - Combined (GAN + TrivialAugment)
- **Explainable AI (XAI):**
  - LIME for fidelity and feature importance analysis.
  - SHAP for local explanations, sparsity and class-wise contrastivity.
  - Grad-CAM for visualizing attention patterns, sanity checks, SSIM.
- **Evaluation Metrics:**
  - Classification accuracy, F1, Precision, Recall, Confusion Matrix.
  - Explainability metrics (e.g., fidelity, sparsity, sanity checks, class-wise contrastivity).

This project includes the following Jupyter notebooks:

1. [MT_GANs.ipynb](MT_GANs.ipynb) - GAN-based data augmentation (Pix2Pix architecture)
2. [MT_XAI_evaluation.ipynb](MT_XAI_evaluation.ipynb) - Evaluation of Explainable AI methods (LIME, SHAP, Grad-CAM)
3. [MT_evaluation.ipynb](MT_evaluation.ipynb) -  CNN model evaluation (F1, Recall, Precision, Accuracy, and confusion matrices)
4. [MT_models.ipynb](MT_models.ipynb) - TrivialAugment + Model trainings
