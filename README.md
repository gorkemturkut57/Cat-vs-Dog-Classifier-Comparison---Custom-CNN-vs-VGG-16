# 🐾 Cat vs Dog Classifier Comparison | Custom CNN vs VGG-16

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.7%2B-green.svg)](https://www.python.org/downloads/release/python-370/)

## 📋 Project Overview
This project presents a **detailed comparison** between a **custom-designed CNN model** and a **pre-trained VGG-16 model** for classifying cat and dog images.  
Both models are thoroughly evaluated using training/validation performance graphs, confusion matrices, classification reports, and a final comprehensive analysis.

---

## 🚀 Models Overview

### 1. Custom CNN Model
- **Training & Validation**:
  - Steady increase in accuracy with occasional validation drops (signs of overfitting).
  - Loss decreases overall but fluctuates on validation data.
- **Confusion Matrix**:
  - Cats: 18 correct / 2 incorrect
  - Dogs: 15 correct / 5 incorrect
- **Performance**:
  - **Accuracy**: 82.5%
  - **Precision**: Higher for dogs
  - **Recall**: Higher for cats
- **Strengths**:
  - Acceptable accuracy for small-scale projects.
  - Good learning trend overall.
- **Weaknesses**:
  - Validation loss fluctuations.
  - Higher misclassification for dogs.

---

### 2. VGG-16 Model (Transfer Learning)
- **Training & Validation**:
  - Very stable and smooth increase in both training and validation accuracy.
  - Minimal overfitting or underfitting observed.
- **Confusion Matrix**:
  - Cats: 18 correct / 2 incorrect
  - Dogs: 16 correct / 4 incorrect
- **Performance**:
  - **Accuracy**: 85%
  - **Precision**: Higher for dogs
  - **Recall**: Higher for cats
- **Strengths**:
  - Very consistent training and validation curves.
  - High accuracy suitable for real-world use.
- **Weaknesses**:
  - Slightly lower recall for dogs (may miss some dogs).
  - Requires more computational resources and longer training time.

---

## 📊 Final Comparison

| Feature | Custom CNN | VGG-16 |
|:--------|:-----------|:------|
| Accuracy | 82.5% | 85% |
| Stability | Moderate (overfitting signs) | Very stable |
| Training Time | Faster | Slower |
| Model Size | Lightweight | Heavy |
| Practical Use | Prototyping, small datasets | Production-level, real-world use |

---

## 🛠️ Technologies Used
- Python
- TensorFlow / Keras
- Scikit-learn
- Matplotlib

---

## 🎯 Conclusion
- **VGG-16 is clearly superior** in terms of performance, stability, and reliability.
- **Custom CNN** is still valuable for fast experiments and low-resource projects.
- **Choosing the right model** depends on project size, hardware limitations, and specific requirements.
