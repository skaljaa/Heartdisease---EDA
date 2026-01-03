# ❤️ Heart Disease Prediction

A machine learning project to predict heart disease using the Cleveland Heart Disease Dataset.

## 📋 Project Overview

This project analyzes patient data to predict the presence and severity of heart disease using classification algorithms. It was developed as a semester project demonstrating data science workflow from exploration to model evaluation.

## 📊 Dataset

- **Source:** UCI Machine Learning Repository - Cleveland Heart Disease Dataset
- **Year:** 1988
- **Institutions:** Cleveland Clinic Foundation, Hungarian Institute of Cardiology, V.A. Medical Center, University Hospital Zurich
- **Size:** 303 patients, 14 features
- **Purpose:** Early detection of heart disease as an alternative to invasive cardiac catheterization

## 🔍 Features

| Feature | Description |
|---------|-------------|
| age | Age in years |
| sex | Sex (1 = male, 0 = female) |
| cp | Chest pain type (1-4) |
| trestbps | Resting blood pressure (mm Hg) |
| chol | Serum cholesterol (mg/dl) |
| fbs | Fasting blood sugar > 120 mg/dl |
| restecg | Resting ECG results (0-2) |
| thalach | Maximum heart rate achieved |
| exang | Exercise induced angina |
| oldpeak | ST depression induced by exercise |
| slope | Slope of peak exercise ST segment |
| ca | Number of major vessels (0-3) |
| thal | Thalassemia type |
| num | **Target:** Diagnosis (0 = healthy, 1-4 = disease severity) |

## 🛠️ Project Steps

1. **Exploratory Data Analysis (EDA)**
   - Dataset structure and statistics
   - 5 statistical questions answered
   - Correlation analysis

2. **Visualization**
   - Scatter plots
   - Correlation heatmap
   - Pairplot
   - Count plots
   - Box plots for outliers

3. **Data Preprocessing**
   - Outlier detection and handling (IQR method)
   - Missing value treatment
   - Feature scaling (StandardScaler)

4. **Classification Models**
   - Logistic Regression
   - K-Nearest Neighbors (KNN)
   - Hyperparameter tuning

## 📈 Results

| Model | Multi-class Accuracy | Binary Accuracy |
|-------|---------------------|-----------------|
| Logistic Regression | 63.9% | 80.3% |
| KNN (K=3) | 63.9% | **85.2%** |

**Best Model:** KNN with K=3 (Binary Classification) - 85.2% accuracy

## 🔑 Key Findings

- Binary classification outperforms multi-class by ~20%
- Key predictors: chest pain type, exercise-induced angina, ST depression, number of vessels
- Males show higher disease rates in the dataset
- Class imbalance affects multi-class performance

## 🧰 Technologies Used

- Python 3.12
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Missingno

## 📁 Project Structure

```
├── HeartDisease.ipynb    # Main Jupyter notebook
├── README.md             # Project documentation
```

## 🚀 Future Improvements

- Collect more data for minority classes
- Try ensemble methods (Random Forest, XGBoost)
- Apply SMOTE for class balancing
- Feature engineering

## 👤 Author

Semester Project - Machine Learning Classification

## 📄 License

This project is for educational purposes.