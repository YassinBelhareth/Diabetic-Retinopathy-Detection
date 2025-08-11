# 🩺 Diabetic Retinopathy Detection with Deep Learning

This repository contains a complete pipeline for detecting **diabetic retinopathy (DR)** from retinal fundus images using deep learning.  
It is based on the **APTOS 2019 Blindness Detection** dataset (Kaggle) and includes multiple state-of-the-art computer vision models and evaluation strategies.

---

## 🎯 Objective
Given a retinal fundus image, classify it into one of the five DR severity levels:

| Label | Description         |
|-------|--------------------|
| 0     | No DR               |
| 1     | Mild                |
| 2     | Moderate            |
| 3     | Severe              |
| 4     | Proliferative DR    |

This is an **ordinal classification** task — classes have a natural order, and misclassifications far apart in severity are penalized more heavily.

---

## 🚀 Features
- **EfficientNetV2-S** for baseline classification
- **Vision Transformer (ViT)** for model comparison
- **Ordinal regression (CORN)** for severity modeling
- Data augmentation optimized for retinal fundus images
- Robust evaluation using **Quadratic Weighted Kappa (QWK)**
- Tuned decision thresholds for optimal performance

---

## 📂 Project Structure
```
Diabetic Retinopathy Detection/
│
├── Diabetic_Retinopathy_Detection.ipynb  # Main Jupyter Notebook
├── README.md                             # Project documentation
└── requirements.txt                      # Dependencies list
```

---

## 📦 Installation
```bash
# Clone this repository
git clone https://github.com/<YOUR_USERNAME>/Diabetic-Retinopathy-Detection.git
cd Diabetic-Retinopathy-Detection

# Install required packages
pip install -r requirements.txt
```

---

## 📊 Dataset
We use the **APTOS 2019 Blindness Detection** dataset from Kaggle.  
[Download here](https://www.kaggle.com/competitions/aptos2019-blindness-detection/data) and place the files in the designated folder inside the project.

---

## 🖥 Usage
1. Open the notebook in Jupyter or Google Colab:
   ```bash
   jupyter notebook Diabetic_Retinopathy_Detection.ipynb
   ```
2. Adjust dataset paths as needed.
3. Run all cells to train and evaluate models.

---

## 📈 Results
- **Best Model**: EfficientNetV2-S with tuned thresholds
- **Metric**: Quadratic Weighted Kappa (QWK)
- Achieved competitive QWK score on validation and test sets.



