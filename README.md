# Binary Mitosis Classification using Deep Learning

## What’s This About?

In histopathology, mitosis detection plays a critical role in understanding how rapidly cells are dividing, which is especially relevant in cancer diagnosis. Among different mitotic figures, atypical mitosis (AMF) serves as a strong marker for tumor aggression and malignancy.

This project focuses on building a binary classifier that differentiates between:

- Normal Mitosis Figures (NMF)
- Atypical Mitosis Figures (AMF)

We implement two widely used convolutional neural network (CNN) architectures—MobileNetV2 and ResNet—to address this binary classification problem using the MIDOG 2025 dataset. The dataset presents typical challenges such as class imbalance and subtle visual differences between classes.

---

## Dataset

- **Source**: [MIDOG 2025 Atypical Mitosis Dataset](https://imig.science/midog25/)
- **Classes**:  
  - AMF (Atypical Mitosis)  
  - NMF (Normal Mitosis)  
- **Challenges**:
  - Significant class imbalance (AMF is underrepresented)
  - Subtle morphological differences that are difficult to distinguish visually
  - Variability in image resolution and quality

---

## What’s Inside

1. **Preprocessing**
   - Image normalization
   - Uniform resizing for model input
   - Handling class imbalance through:
     - Weighted loss functions
     - Data augmentation focused on underrepresented AMF class

2. **Model Architectures**
   - MobileNetV2: Lightweight architecture suitable for deployment and efficient inference
   - ResNet18 / ResNet50: Deep residual networks effective in capturing complex patterns

3. **Training Strategy**
   - Loss Function: Binary Cross-Entropy with Class Weights
   - Optimizers: Adam and SGD variants
   - Evaluation Metrics: Accuracy, Precision, Recall, F1 Score, and ROC-AUC

4. **Evaluation**
   - Confusion matrix visualization
   - ROC curve generation
   - Class-wise performance reporting

---
