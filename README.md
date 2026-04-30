# Machine Learning Algorithms & Evaluation Experiments

This repository demonstrates the implementation and analysis of key machine learning algorithms for classification tasks. It includes experiments on model performance, overfitting, hyperparameter tuning, and evaluation techniques.

---

## Project Objectives

- Implement popular classification algorithms
- Compare model performance and generalization
- Analyze overfitting and underfitting
- Tune hyperparameters for optimal results
- Visualize decision boundaries and variance
- Apply proper evaluation metrics and validation methods

---

## Implementations & Experiments

### 1. Decision Tree vs Random Forest
- Implemented Decision Tree and Random Forest classifiers
- Compared accuracy and overfitting behavior

**Key Insight:**
- Decision Trees tend to overfit
- Random Forest improves generalization via ensemble learning

---

### 2. Random Forest Hyperparameter Tuning
- Tuned parameters:
  - `n_estimators`
  - `max_depth`
  - `min_samples_split`
- Used Grid Search / Random Search

**Outcome:**
- Improved model accuracy and reduced overfitting

---

### 3. Support Vector Machine (SVM)
- Implemented SVM with linear kernel
- Visualized decision boundary on 2D dataset

---

### 4. Effect of Regularization Parameter (C)
- Tested different values of `C`

**Observations:**
- Small `C` → smoother boundary (underfitting risk)
- Large `C` → tighter fit (overfitting risk)

---

### 5. KNN Distance Metrics Comparison
- Compared:
  - Euclidean Distance
  - Manhattan Distance

**Conclusion:**
- Performance varies based on dataset geometry

---

### 6. Feature Scaling in KNN
- Applied scaling on 3D dataset

**Result:**
- Significant improvement in model performance

---

### 7. PCA (Principal Component Analysis)
- Plotted explained variance ratio
- Determined optimal number of components

---

### 8. 📉 Model Evaluation Metrics
- Confusion Matrix
- Precision
- Recall
- F1-score

---

### 9. Cross Validation vs Train-Test Split
- Implemented k-fold cross-validation

**Observation:**
- Cross-validation provides more reliable results

---

### 10. KNN with Different K Values
- Evaluated K values from 3 to 10

**Finding:**
- Optimal K balances bias and variance

---

### 11. Bagging vs Single Model
- Applied Bagging Classifier

**Result:**
- Improved stability and reduced variance

---

## Tech Stack

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## Author 
Vinayak Sharma 
GitHub
https://github.com/vsbeginner

LinkedIn
https://www.linkedin.com/in/vinayak-sharma-24a8aa384/
