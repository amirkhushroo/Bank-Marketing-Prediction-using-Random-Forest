# 🏦 Bank Marketing Analysis and Prediction

## 📌 Project Overview

This project uses Machine Learning to predict whether a customer will subscribe to a bank term deposit based on demographic and campaign-related information.

The model is trained using the **Random Forest Classifier**, which is an ensemble learning algorithm that combines multiple decision trees to improve prediction accuracy and reduce overfitting.

---

## 📂 Dataset

Dataset used:

- cleaned-data.csv

The target variable is:

- **y**
    - yes → Customer subscribed
    - no → Customer did not subscribe

---

## 🎯 Objective

Build a machine learning classification model that predicts whether a customer will subscribe to a bank term deposit.

---

## 🛠 Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn

---

## 📚 Libraries Used

```python
import pandas as pd
import numpy as np

from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score
```

---

## 📊 Project Workflow

### 1. Load Dataset

- Read the cleaned dataset.

### 2. Data Exploration

- Dataset information
- Missing value checking
- Statistical summary

### 3. Feature Selection

Separate features and target variable.

```python
X = df.drop("y", axis=1)
y = df["y"]
```

### 4. Data Encoding

Convert categorical variables into numerical format using One-Hot Encoding.

```python
pd.get_dummies()
```

### 5. Split Dataset

Split the data into training and testing datasets.

- Training Data : 80%
- Testing Data : 20%

### 6. Model Training

Train a Random Forest Classifier.

### 7. Model Evaluation

Evaluate the model using Accuracy Score.

### 8. Prediction

Predict customer subscription for new records.

---

## 🤖 Machine Learning Model

### Random Forest Classifier

Random Forest is an ensemble learning algorithm that creates multiple decision trees and combines their predictions.

### Advantages

- High accuracy
- Handles large datasets
- Reduces overfitting
- Works well with categorical and numerical data

---

## 📈 Evaluation Metric

- Accuracy Score

---

## 📁 Files

| File | Description |
|------|-------------|
| prediction_model(RandomForest).ipynb | Jupyter Notebook |
| cleaned-data.csv | Dataset |
| README.md | Project Documentation |

---

## ▶️ How to Run

### Clone Repository

```bash
git clone https://github.com/yourusername/Bank-Marketing-Analysis-and-Prediction.git
```

### Install Libraries

```bash
pip install pandas numpy scikit-learn notebook
```

### Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```
prediction_model(RandomForest).ipynb
```

Run all cells.

---

## Future Improvements

- Hyperparameter Tuning
- Cross Validation
- Feature Importance Visualization
- Confusion Matrix
- Precision, Recall, F1 Score
- ROC-AUC Curve
- Deploy the model using Flask or Streamlit

---

## Author

Amir Khushroo 

B.Tech CSE (Data Science & AI)

Machine Learning Enthusiast
