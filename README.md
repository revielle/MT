# MT

This repository contains the code and resources for a brain tumor classification project using deep learning. The study explores the impact of data augmentation and explainable AI (XAI) techniques, such as LIME, SHAP, and Grad-CAM, to improve performance and interpretability.

## Features
- **Multi-class Brain Tumor Classification:** Glioma, Meningioma, Pituitary Tumor, and No Tumor.
- **Data Augmentation:** 
  - Traditional (e.g., TrivialAugment)
  - Generative (GAN-based synthetic data)
- **Explainable AI (XAI):**
  - LIME for fidelity and feature importance analysis.
  - SHAP for sparsity and local explanations.
  - Grad-CAM for visualizing attention patterns.
- **Evaluation Metrics:**
  - Classification accuracy.
  - Explainability metrics (e.g., fidelity, sparsity, class-wise contrastivity).


## Augmentation Techniques
1. **TrivialAugment**: A search-based augmentation method that applies simple transformations like rotation, flipping, and color adjustments.
2. **GAN-based Augmentation**: Generative Adversarial Networks (GANs) were used to synthesize realistic tumor images, addressing class imbalances and data scarcity.

## Explainable AI Methods
1. **LIME (Local Interpretable Model-agnostic Explanations):**
   - Used to analyze the fidelity of model predictions and feature relevance.
2. **SHAP (SHapley Additive exPlanations):**
   - Provides pixel-level explanations for feature importance.
3. **Grad-CAM (Gradient-weighted Class Activation Mapping):**
   - Visualizes regions of an image the model focuses on during predictions.
  
## Results
### Performance Metrics
- **TrivialAugment Model:** Test Accuracy: **94.43%**
- **GAN-Augmented Model:** Test Accuracy: **93.82%**
- **Baseline Model:** Test Accuracy: **92.30%**

### Explainability Metrics
- **Fidelity Scores (LIME):** TrivialAugment (0.809), GAN (0.719), Baseline (0.608)
- **Sparsity Scores (SHAP):** TrivialAugment (0.845), GAN (0.793)
- **Focused Attention (Grad-CAM Coverage):** TrivialAugment (2.49%), GAN (3.79%), Baseline (4.41%)

