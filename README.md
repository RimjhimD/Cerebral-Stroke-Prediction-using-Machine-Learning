# 🧠 MACHINE LEARNING LABORATORY PROJECT  
### Course Code: CSE 4312 | Semester: 7th  

---

## 📌 Course Information
- **Course Title:** Machine Learning Laboratory  
- **Course Code:** CSE 4312  
- **Instructor:** MD Tamim Hossain  
- **Designation:** Lecturer  
- **Department:** Computer Science and Engineering  

---

## 👥 Team Members
- **MD Nishadul Islam** (0222220005101014)  
- **Tahsin Ahmed** (0222220005101017)  
- **Rimjhim Dey** (0222220005101039)  

---

## 💻 Development Platform
This project was developed collaboratively using **Google Colab**, enabling efficient experimentation, visualization, and model training in a cloud-based environment.

---

## 📖 Project Overview
This project demonstrates a **complete end-to-end Machine Learning pipeline**, covering all essential stages from data collection to model optimization.

### 🎯 Objectives
- Data preprocessing and cleaning  
- Feature engineering and selection  
- Model building and evaluation  
- Handling imbalanced datasets  
- Neural network implementation  
- Hyperparameter tuning  

---

## ⚙️ Setup Instructions

### 🔹 1. Clone the Repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 🔹 2. Install Required Libraries
```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost imbalanced-learn tensorflow torch optuna
```

### 🔹 3. Run the Project
- Open the notebook in **Google Colab** or **Jupyter Notebook**
- Run all cells step by step

---

## 🚀 Project Workflow (Step-by-Step)

### 🔹 Step 1: Library Setup
Imported essential libraries:
- NumPy, Pandas → data handling  
- Matplotlib, Seaborn → visualization  
- Scikit-learn → ML models  
- TensorFlow, PyTorch → deep learning  
- Imbalanced-learn → class imbalance handling  

---

### 🔹 Step 2: Data Collection & Loading
- Dataset collected from Kaggle  
- Loaded into Pandas DataFrame  
- Used as the base for analysis  

---

### 🔹 Step 3: Exploratory Data Analysis (EDA)
- Checked dataset structure (`head`, `info`, `shape`)  
- Generated statistical summary (`describe`)  
- Identified numerical & categorical features  
- Detected missing values  
- Visualized:
  - Outliers (boxplots)  
  - Correlations (heatmap)  
  - Data distribution & skewness  
- Checked for duplicates  

---

### 🔹 Step 4: Data Preprocessing
- **Missing Values Handling**
  - Numerical → mean  
  - Categorical → mode  

- **Outlier Treatment**
  - Z-score method  
  - Percentile capping  

- **Encoding**
  - One-Hot Encoding  
  - Target Encoding  

- **Feature Selection**
  - Removed correlated features  
  - Used Random Forest importance  

- **Feature Scaling**
  - Standardization (StandardScaler)  
  - Normalization (Min-Max)  

- **Data Splitting**
  - Train-test split (stratified)  

---

### 🔹 Step 5: Feature Selection Techniques
Applied:
- Pearson Correlation  
- Variance Threshold  
- Mutual Information  
- Chi-Square Test  

Evaluated using Linear Regression (MSE & R²).

---

### 🔹 Step 6: Logistic Regression Model
- Built classification model  
- Trained and predicted  
- Evaluated using:
  - Confusion Matrix  
  - Accuracy  
  - Precision & Recall  
  - ROC-AUC Curve  

⚠️ Observed poor performance for minority class.

---

### 🔹 Step 7: Model Analysis & Class Imbalance Handling
- Analyzed bias and variance  
- Identified underfitting issues  
- Applied **SMOTE**  
- Improved recall for minority class  

---

### 🔹 Step 8: Overfitting & Regularization
Applied:
- L1 Regularization  
- L2 Regularization  
- Elastic Net  
- Early Stopping  

Compared model generalization performance.

---

### 🔹 Step 9: Neural Network Implementation
Implemented using:
- NumPy (from scratch)  
- TensorFlow / Keras  
- PyTorch  

Compared performance and complexity.

---

### 🔹 Step 10: Model Complexity Analysis
- Increased neurons (widening)  
- Increased layers (deepening)  

Observed impact on loss and accuracy.

---

### 🔹 Step 11: Backpropagation
- Forward pass and loss calculation  
- Gradient computation  
- Weight updates  
- Performance visualization  

---

### 🔹 Step 12: Hyperparameter Tuning
Applied:
- Grid Search  
- Random Search  
- Bayesian Optimization (Optuna)  

Used **Stratified K-Fold Cross Validation**.

---

## 📊 Tools & Technologies
- Python  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- Scikit-learn  
- TensorFlow / Keras  
- PyTorch  
- XGBoost  
- Imbalanced-learn  
- Optuna  

---

## 🎯 Key Outcomes
- Built complete ML pipeline  
- Solved real-world data issues  
- Improved model performance  
- Compared multiple frameworks  

---

## 📁 Project Structure
```
├── data/
├── notebooks/
├── models/
├── results/
├── README.md
```

---

## 📌 Conclusion
This project provides a strong understanding of **machine learning workflows**, from preprocessing to advanced optimization, combining theory and practical implementation.

---

## 🙏 Acknowledgment
We sincerely thank **MD Tamim Hossain** for his guidance and support throughout this course.

---
