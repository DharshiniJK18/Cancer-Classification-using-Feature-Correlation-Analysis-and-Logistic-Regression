# Breast Cancer Classification using Feature Analysis and Logistic Regression

## 📌 Overview
This project focuses on classifying breast tumors as **benign** or **malignant** using machine learning techniques. The analysis includes data preprocessing, visualization, feature correlation analysis, and model building using Logistic Regression.

---

## 📂 Dataset
- **Name:** Breast Cancer Wisconsin (Diagnostic) Dataset  
- **Source:** UCI Machine Learning Repository  
- **Samples:** 569  
- **Features:** 30 numerical features derived from digitized images of breast mass cell nuclei  

### 🧬 Target Variable
- `diagnosis`
  - 0 → Benign  
  - 1 → Malignant  

---

## ⚙️ Workflow

### 1. Data Preprocessing
- Removed unnecessary column (`Unnamed: 32`)
- Checked for missing values
- Encoded categorical variable (`diagnosis`) using Label Encoding

### 2. Exploratory Data Analysis
- Count plot to visualize class distribution
- Correlation heatmap to identify relationships between features
- Pair plot to observe feature interactions and class separation

### 3. Feature Selection
- Removed ID column
- Selected relevant numerical features for model training

### 4. Data Splitting
- Training set: 80%  
- Testing set: 20%

### 5. Feature Scaling
- Applied StandardScaler to normalize feature values

### 6. Model Building
- Algorithm: Logistic Regression
- Trained on scaled training data

---

## Results

- **Training Accuracy:** ~98.9%  
- **Testing Accuracy:** ~95.6%  

###  Classification Report
- High precision and recall for both benign and malignant classes
- Balanced performance across classes

---

## 🔍 Key Insights
- Strong correlation observed between features like `radius_mean`, `perimeter_mean`, and `area_mean`
- Certain features show strong influence on diagnosis prediction
- Presence of multicollinearity suggests redundancy in features
- Model performs well due to clear separation between classes

---

## ⚠️ Limitations
- Multicollinearity among features may affect model interpretability
- No feature reduction techniques (e.g., PCA) applied
- Model performance may vary with different datasets

---

##  Future Improvements
- Apply feature selection or dimensionality reduction (PCA)
- Try advanced models (Random Forest, SVM, Neural Networks)
- Perform cross-validation for more robust evaluation

---

##  Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📎 Conclusion
This project demonstrates how machine learning can effectively classify breast cancer tumors using feature-based analysis. Logistic Regression provides high accuracy, supported by strong feature correlations and clear class separability.

---

## 👩‍💻 Author
- *Your Name*
