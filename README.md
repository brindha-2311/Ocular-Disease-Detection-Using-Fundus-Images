🩺 Ocular Disease Detection Using Fundus Images

Automated detection of retinal diseases is a critical step toward preventing avoidable blindness and improving clinical decision-making in ophthalmology.
This project presents a deep learning–based multi-class retinal disease classification system using fundus images, targeting:

Cataract (CA)

Diabetic Retinopathy (DR)

Glaucoma (GL)

Normal

A total of 4,217 fundus images from publicly available datasets were preprocessed using CLAHE, Wavelet Transform, and Blood Vessel Segmentation to enhance structural and contrast features.

Multiple architectures — VGG19, ResNet50, Vision Transformer (ViT), Graph Neural Network (GNN), and EfficientNet-B0 — were trained and evaluated using 5-fold cross-validation.
Among these, EfficientNet-B0 achieved the best performance:

Accuracy: 93.83%

Precision: 0.94

Recall: 0.94

F1-Score: 0.94

To ensure interpretability and clinical reliability, several Explainable AI (XAI) techniques were applied, including:

LIME, Grad-CAM, Integrated Gradients, Gradient SHAP, Guided Backpropagation, Saliency Maps, and Occlusion Sensitivity.

Visualization results show that the models focused on clinically meaningful retinal regions, demonstrating transparency and trustworthiness.
The proposed EfficientNet-B0–based system delivers strong diagnostic accuracy, stability, and interpretability — making it a promising tool for automated retinal disease screening.

📁 Project Structure
Ocular-Disease-Detection-Using-Fundus-Images/
│
├── ConvNeXt_Model.ipynb                 # ConvNeXt full training pipeline (separate file)
│
├── MultiModel_XAI.ipynb                 # VGG19 + ResNet50 + ViT + GNN + EfficientNet-B0 all XAI methods
│                                        # Contains training, evaluation, confusion matrices,
│                                        # accuracy curves, and XAI visualizations
│
├── EfficientNetB0_Model.ipynb           # Best-performing model (separate file)
│                                        # Includes preprocessing + training + 5-fold CV
│
└── README.md

🚀 Features
✔ ConvNeXt Model (Separate File)

Full training pipeline

Augmentation & preprocessing

Evaluation (accuracy, loss, confusion matrix)

Achieved 90.64% accuracy

✔ Combined Multi-Model Notebook

Includes:

VGG19

ResNet50

EfficientNet-B0

Vision Transformer (ViT)

Graph Neural Network (GNN)

All XAI Visualizations

Features:

Preprocessing (CLAHE + Wavelet + Vessel Segmentation)

Model training & validation

Accuracy and loss plots

Confusion matrices

XAI heatmaps for model interpretability

✔ EfficientNet-B0 (Separate File — Best Model)

5-fold cross-validation

Best performing model with 93.83% accuracy

Highly robust & clinically interpretable

Extended XAI interpretation layer

🛠️ Technologies Used

Python

PyTorch / TensorFlow

OpenCV

NumPy / Pandas

scikit-learn

Matplotlib / Seaborn

Jupyter Notebook

📊 Model Performance Summary
Model	Accuracy	Notes
EfficientNet-B0	93.83%	Best performance (separate file)
ConvNeXt	90.64%	Separate notebook
VGG19	88.51%	Part of combined notebook
ResNet50	~89–92%	Combined notebook
Vision Transformer (ViT)	~90%	Combined notebook
Graph Neural Network (GNN)	Structure-based learning	Combined notebook

Confusion matrices, accuracy curves, and XAI plots are included in each notebook.

🧠 Explainable AI (XAI) Methods Used

To build clinical trust:

Grad-CAM

Integrated Gradients

LIME

Gradient SHAP

Guided Backpropagation

Saliency Maps

Occlusion Sensitivity

These methods highlight retinal areas contributing to predictions, confirming clinical relevance.

✅ Conclusion

This project provides a complete deep learning pipeline for retinal disease detection with:

High diagnostic accuracy

Strong generalization across folds

Clinically meaningful explainability

Multiple deep learning architectures

Best performance achieved by EfficientNet-B0

The system is suitable for automated screening, clinical decision support, and research applications.
