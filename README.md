# Improving Model Generalization of Pneumonia Detection from Chest X-ray Images

This repository contains my MSc dissertation project for the MSc Software Engineering and Artificial Intelligence degree.  
The project focuses on improving the **generalization performance** of deep learning models for pneumonia detection using chest X-ray images by applying **transfer learning** and **cross-dataset evaluation**.

---

## 📌 Project Overview
Pneumonia remains a major global health concern, and chest X-rays are widely used for diagnosis.  
While deep learning models achieve high accuracy on familiar datasets, they often struggle to generalize to unseen clinical data.

This project addresses that challenge by:
- Using **transfer learning**
- Evaluating models on **external unseen datasets**
- Comparing model robustness across datasets

---

## 🎯 Research Objectives
- Apply transfer learning for pneumonia detection using chest X-ray images  
- Compare the generalization ability of **ResNet152** and **DenseNet201**
- Evaluate performance using standard medical imaging metrics
- Validate models on an **independent external dataset**

---

## 🧠 Models Used
- **DenseNet201** (ImageNet pretrained)
- **ResNet152** (ImageNet pretrained)

Both models were fine-tuned using:
- Layer freezing and unfreezing
- Learning rate optimization
- Data augmentation strategies

---

## 📊 Datasets
Publicly available chest X-ray datasets were used:

- COVID-19 Radiography Database  
- Chest X-ray (COVID-19 & Pneumonia) Dataset  
- External unseen dataset for generalization testing  

All images were resized to **224×224** and normalized before training.

---

## 📈 Evaluation Metrics
Model performance was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix analysis

---

## 🔬 Key Results
- **DenseNet201** achieved superior performance and generalization:
  - 93.2% accuracy (AUC = 0.9916) on the main dataset
  - 88.3% accuracy (AUC = 0.9742) on unseen data
- DenseNet201 consistently outperformed ResNet152 across datasets
- Most classification errors occurred between *Normal* and *Pneumonia*, reflecting real-world diagnostic challenges

---

## 🛠 Tools & Technologies
- Python 3
- TensorFlow / Keras
- Google Colab
- NumPy, Pandas
- Matplotlib, scikit-learn
- OpenCV

---

## 📂 Repository Structure

