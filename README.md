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

The primary goal was to understand and implement:
- Data preprocessing techniques  
- Feature engineering and selection  
- Model building and evaluation  
- Handling imbalanced datasets  
- Neural network implementation  
- Hyperparameter tuning  

---

## ⚙️ Setup Instructions

### 🔹 1. Clone the Repository

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

🔹 2. Install Required Libraries
pip install numpy pandas matplotlib seaborn scikit-learn xgboost imbalanced-learn tensorflow torch optuna
🔹 3. Run the Project
Open the notebook in Google Colab or Jupyter Notebook
Execute cells step by step
🚀 Project Workflow (Step-by-Step)
🔹 Step 1: Library Setup

Imported essential libraries such as:

NumPy and Pandas for data manipulation
Matplotlib and Seaborn for visualization
Scikit-learn for machine learning models
TensorFlow, PyTorch for deep learning
Imbalanced-learn for handling class imbalance
🔹 Step 2: Data Collection & Loading
Dataset collected from Kaggle
Loaded into a Pandas DataFrame
Served as the foundation for all analysis
🔹 Step 3: Exploratory Data Analysis (EDA)

Performed detailed analysis to understand the dataset:

Checked structure using df.head(), df.info(), df.shape
Generated statistical summaries (df.describe())
Identified numerical and categorical features
Detected missing values
Visualized:
Outliers using boxplots
Correlations using heatmaps
Feature distributions and skewness
Verified data integrity (no duplicates)
🔹 Step 4: Data Preprocessing

Prepared data for modeling:

Missing Values Handling:
Numerical → mean imputation
Categorical → mode imputation
Outlier Treatment:
Z-score method
Capping using percentiles
Encoding Techniques:
One-Hot Encoding for nominal features
Target Encoding for specific variables
Feature Selection:
Removed highly correlated features
Used Random Forest for feature importance
Feature Scaling:
Standardization (StandardScaler)
Normalization (Min-Max Scaling)
Data Splitting:
Train-test split with stratification
🔹 Step 5: Feature Selection Techniques

Applied filter-based methods:

Pearson Correlation
Variance Threshold
Mutual Information
Chi-Square Test

Evaluated impact using Linear Regression (MSE & R²).

🔹 Step 6: Logistic Regression Model
Built classification model
Performed training and prediction
Evaluated using:
Confusion Matrix
Accuracy
Precision & Recall
ROC-AUC Curve

Identified poor minority class performance due to imbalance.

🔹 Step 7: Model Analysis & Class Imbalance Handling
Analyzed bias and variance
Demonstrated underfitting and model limitations
Applied SMOTE (Synthetic Minority Oversampling Technique)
Improved recall significantly for minority class
🔹 Step 8: Overfitting & Regularization

Conducted controlled experiments:

Forced overfitting using deep neural network
Applied:
L1 Regularization
L2 Regularization
Elastic Net
Early Stopping

Compared performance improvements and generalization.

🔹 Step 9: Neural Network Implementation

Implemented neural networks using:

NumPy: From scratch (manual forward & backpropagation)
TensorFlow/Keras: High-level API
PyTorch: Flexible deep learning framework

Compared performance, complexity, and results.

🔹 Step 10: Model Complexity Analysis

Explored:

Widening: Increasing neurons
Deepening: Increasing layers

Observed impact on model performance and loss.

🔹 Step 11: Backpropagation
Explained forward pass and loss calculation
Implemented gradient computation
Updated weights using optimization techniques
Visualized training performance
🔹 Step 12: Hyperparameter Tuning

Optimized models using:

Grid Search
Random Search
Bayesian Optimization (Optuna)

Used Stratified K-Fold Cross-Validation for robust evaluation.

📊 Tools & Technologies
Python
NumPy, Pandas
Matplotlib, Seaborn
Scikit-learn
TensorFlow / Keras
PyTorch
XGBoost
Imbalanced-learn
Optuna
🎯 Key Outcomes
Built a complete ML pipeline
Handled real-world challenges like missing data and imbalance
Improved model performance using advanced techniques
Compared multiple ML and deep learning frameworks
📁 Project Structure
├── data/
├── notebooks/
├── models/
├── results/
├── README.md
📌 Conclusion

This project provides a comprehensive understanding of machine learning workflows, from data preprocessing to advanced model optimization, combining both theoretical knowledge and practical implementation.

🙏 Acknowledgment

We would like to express our sincere gratitude to MD Tamim Hossain for his guidance and support throughout this course.


---

