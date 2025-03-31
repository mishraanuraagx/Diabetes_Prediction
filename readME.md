## 🩺 Diabetes Prediction with Machine Learning
📘 Introduction

The Diabetes Prediction Dataset is a collection of medical and demographic data from patients, along with their diabetes status (positive or negative). The data includes features such as:

- Age
- Gender
- Body Mass Index (BMI)
- Hypertension
- Heart Disease
- Smoking History
- HbA1c Level
- Blood Glucose Level

This dataset is ideal for building machine learning models to predict diabetes based on a patient's history and profile. Such models can assist healthcare professionals in:

### Identifying at-risk individuals

Creating personalized treatment plans

Understanding the impact of different features on diabetes likelihood

📊 Dataset sourced from a Kaggle challenge.

## ⚙️ Environment Setup
```bash
conda create -n diabetes_env python=3.10
conda activate diabetes_env
pip install numpy pandas matplotlib seaborn scikit-learn imbalanced-learn jupyter
```
## 💻 Code & Dataset Analysis
All code and model development is documented in the notebook:

📁 diabetes_prediction.ipynb

## 📊 Visual Reference
### 🔗 Correlation Heatmap
![corrs.png](images%2Fcorrs.png)

### ⚠️ Original Dataset: Imbalanced
![imbalanced_target.png](images%2Fimbalanced_target.png)

### 📈 Histograms of Numerical Features
![numerical_dataset_hist.png](images%2Fnumerical_dataset_hist.png)

### 🤖 Comparison of Different Models
![model_comparison.png](images%2Fmodel_comparison.png)

## 🏆 Model Selection

🥇 Best Overall: Random Forest
- Accuracy: 0.9672

- Precision: 0.9357

- Recall: 0.6594

- AUC: 0.8276

- F1-score: 0.7736

Random Forest provides the best balance across all performance metrics.

### 🔍 Others:
Decision Tree slightly outperforms Logistic Regression.

It also has the best AUC among all models.

### 📏 Why Every Metric Matters
In imbalanced classification problems:

### 🚫 Avoid Relying Only On:
- Accuracy: Can be misleading

- Plain F1-score: Especially if not macro or weighted

✅ Use Instead:
- Recall or Precision-Recall AUC: Crucial for minority class detection

- Macro F1-score: To evaluate both classes equally

- AUC-PR: Better than ROC-AUC when class imbalance is severe

🔬 Further Research
Consider experimenting with other models:

- AdaBoost

- Gradient Boosting

⚠️ While these can improve accuracy, they often reduce interpretability.