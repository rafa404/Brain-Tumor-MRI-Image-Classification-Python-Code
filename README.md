# Brain Tumor MRI Image Classification

### 🧾 Paper:
**Comparative Analysis of Deep Learning Architectures for Brain Tumor Classification using MRI Images**  
*Accepted at CONMEDIA 2025*

---

## 📖 Description

This repository contains Jupyter Notebook implementations used in our research paper accepted at **CONMEDIA 2025**, titled *“Comparative Analysis of Deep Learning Architectures for Brain Tumor Classification using MRI Images.”*

The project focuses on evaluating and comparing multiple deep learning architectures for accurate brain tumor detection using MRI images. Each notebook in this repository corresponds to a specific model and demonstrates the full workflow — from data preprocessing to training, evaluation, and visualization.

---

## 🧩 Models Implemented
The following CNN-based architectures were explored and compared:

- **VGG16 / VGG19**  
- **ResNet50 / ResNet152**  
- **DenseNet121 / DenseNet201**  
- **InceptionV3**  
- **EfficientNet-B4 / EfficientNet-B7**  
- **Custom CNN-7** (lightweight baseline)

---

## 🧠 Dataset
We used the **Brain Tumor MRI Dataset** from Kaggle:  
📦 [https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)

The dataset includes four MRI image classes:
- **Glioma Tumor**
- **Meningioma Tumor**
- **Pituitary Tumor**
- **No Tumor**

Each image was resized, normalized, and augmented to improve generalization and prevent overfitting.

---

## ⚙️ Methodology
Each notebook follows this general pipeline:

1. **Data Loading & Preprocessing**
   - Resizing to `224x224`
   - Normalization (mean/std)
   - Data augmentation (flip, rotation, zoom)

2. **Model Selection & Training**
   - Transfer learning using ImageNet-pretrained models
   - Fine-tuning last few layers
   - Optimizer: Adam  
   - Loss: Categorical Cross-Entropy  

3. **Evaluation**
   - Accuracy, Precision, Recall, and F1-score
   - Confusion Matrix and ROC-AUC curves
   - Grad-CAM visualizations for interpretability

---

## 🧾 Key Findings
| Model | Accuracy (%) | Precision | Recall | F1-Score |
|--------|---------------|------------|---------|-----------|
| DenseNet121 | **99.85** | 0.99 | 0.99 | 0.99 |
| InceptionV3 | **99.85** | 0.99 | 0.99 | 0.99 |
| DenseNet201 | 99.31 | 0.99 | 0.99 | 0.99 |
| ResNet152 | 99.08 | 0.98 | 0.99 | 0.99 |

**DenseNet121** and **InceptionV3** demonstrated the best balance between accuracy and computational efficiency.

---

## 📊 Results Overview
- Achieved **≈99.8% accuracy** on test data.
- Models consistently reached near-perfect precision, recall, and F1-score.
- Transfer learning significantly improved performance over standard CNNs.
- Lightweight **Custom CNN-7** provided competitive results for real-time use.

---

## 💡 Conclusion
This study highlights the effectiveness of CNN architectures and transfer learning for reliable brain tumor classification using MRI scans. The findings underscore the potential of deep learning models in aiding radiologists for early tumor detection and diagnosis.

---

## 📚 Citation
If you use this repository, please cite our paper:

