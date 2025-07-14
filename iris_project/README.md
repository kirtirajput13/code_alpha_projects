# 🌸 Iris Flower Classification | CodeAlpha Internship Project

This project is part of my internship at **CodeAlpha**, where I built a machine learning model to classify different species of iris flowers using their petal and sepal dimensions.

## 📌 Objective
To predict the species of an iris flower — *Setosa*, *Versicolor*, or *Virginica* — based on its:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

## 🚀 Tools & Technologies
- **Python**
- **Scikit-learn** (for ML model)
- **Pandas** (for data handling)
- **NumPy** (for numeric operations)
- **Seaborn & Matplotlib** (for data visualization)

## 📁 Dataset

The dataset used is [`Iris.csv`](https://archive.ics.uci.edu/ml/datasets/iris), containing 150 flower samples with 4 features:

- `SepalLengthCm`
- `SepalWidthCm`
- `PetalLengthCm`
- `PetalWidthCm`
- `Species` (target class: Setosa, Versicolor, Virginica)

---

## ✅ Project Workflow

### 1. **Data Preprocessing**
- Dropped `Id` column
- Encoded categorical target (`Species`) using `LabelEncoder`
- Standardized features using `StandardScaler`

### 2. **Model Training**
- Trained 3 classifiers:
  - Logistic Regression
  - Support Vector Machine (SVM)
  - Random Forest Classifier
- Performed `train_test_split` with stratification

### 3. **Evaluation**
- Used:
  - Accuracy Score
  - Classification Report
  - Confusion Matrix (with visualizations)
  - 5-Fold Cross-Validation

### 4. **Feature Importance**
- Extracted from the trained Random Forest model and visualized with a barplot

### 5. **Visualization**
- Generated a `pairplot` colored by species for data insight

### 6. **Model Saving**
- Saved the final Random Forest model and the scaler using `joblib`:
  - `iris_rf_model.pkl`
  - `iris_scaler.pkl`

---

## 🔧 How to Run

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/iris-flower-classification.git
cd iris-flower-classification
