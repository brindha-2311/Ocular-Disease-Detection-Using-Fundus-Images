
# 🩺 Ocular Disease Detection Using Fundus Images

Automated detection of retinal diseases is a critical step toward preventing avoidable blindness and improving clinical decision-making in ophthalmology.
This project presents a **deep learning–based multi-class retinal disease classification system** using fundus images, targeting the following classes:

* **Cataract (CA)**
* **Diabetic Retinopathy (DR)**
* **Glaucoma (GL)**
* **Normal**

A total of **4,217 fundus images** from publicly available datasets were preprocessed using:

* **CLAHE (Contrast Limited Adaptive Histogram Equalization)**
* **Wavelet Transform**
* **Blood Vessel Segmentation**

These techniques enhance structural clarity and contrast for optimal model learning.

Multiple deep learning architectures — **VGG19, ResNet50, Vision Transformer (ViT), Graph Neural Network (GNN), and EfficientNet-B0** — were trained and evaluated using **5-fold cross-validation**.

Among all models, **EfficientNet-B0** achieved the highest performance:

* **Accuracy:** 93.83%
* **Precision:** 0.94
* **Recall:** 0.94
* **F1-Score:** 0.94

To ensure interpretability and clinical reliability, several Explainable AI (XAI) techniques were used:

**LIME, Grad-CAM, Integrated Gradients, Gradient SHAP, Guided Backpropagation, Saliency Maps, and Occlusion Sensitivity.**

The model visualizations show that the network focuses on clinically meaningful retinal regions, providing transparent and trustworthy predictions.

The proposed **EfficientNet-B0–based system** demonstrates strong diagnostic accuracy, robustness, and interpretability — making it a promising tool for automated retinal disease screening and early diagnosis.

---

## 🚀 Features

### ✔ **ConvNeXt Model (Separate File)**

* Full training pipeline
* Preprocessing & augmentation
* Evaluation metrics: accuracy, loss, confusion matrix
* Achieved **90.64% accuracy**

---

### ✔ **Combined Multi-Model + XAI Notebook**

Includes implementation of:

* **VGG19**
* **ResNet50**
* **EfficientNet-B0**
* **Vision Transformer (ViT)**
* **Graph Neural Network (GNN)**
* **All XAI Techniques**

Features:

* Preprocessing (CLAHE + Wavelet + Vessel Segmentation)
* Model training & validation
* Accuracy/loss plots
* Confusion matrices
* XAI heatmaps for explainability

---

### ✔ **EfficientNet-B0 (Separate File — Best Model)**

* Full pipeline with preprocessing
* **5-fold cross-validation**
* Best performance: **93.83% accuracy**
* Most stable and clinically interpretable
* Extended XAI analysis

---

## 🛠️ Technologies Used

* **Python**
* **PyTorch / TensorFlow**
* **OpenCV**
* **NumPy / Pandas**
* **scikit-learn**
* **Matplotlib / Seaborn**
* **Jupyter Notebook**

All notebooks include confusion matrices, accuracy/loss graphs, and XAI outputs.

---

## 🧠 Explainable AI (XAI) Methods Used

XAI enhances clinical trust and interpretability using:

* **Grad-CAM**
* **Integrated Gradients**
* **LIME**
* **Gradient SHAP**
* **Guided Backpropagation**
* **Saliency Maps**
* **Occlusion Sensitivity**

These methods highlight retinal areas influencing predictions, confirming medical relevance.

---

## ✅ Conclusion

This project provides a comprehensive deep learning pipeline for retinal disease detection featuring:

* High diagnostic accuracy
* Strong generalization via 5-fold CV
* Clinical explainability with XAI
* Multiple advanced architectures
* Best overall performance using EfficientNet-B0

The system is well-suited for:

* **Automated disease screening**
* **Clinical decision support**
* **Research and academic studies**
* **Real-world ophthalmology AI applications**

