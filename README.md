<div align="center">

# Advanced Machine Learning Algorithms & Evaluation Experiments
### Empirical Comparison of Ensembles, Kernel SVMs, Distance Metrics & Dimensionality Reduction

[![Python](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-3776AB.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E.svg?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626.svg?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243.svg?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

<p align="center">
  <b>A comprehensive empirical investigation of core machine learning algorithms, bias-variance tradeoffs, and statistical validation methodologies.</b><br>
  Covering Random Forests, Bagging Ensembles, Support Vector Machines, K-Nearest Neighbors metric geometries, PCA manifold reductions, and stratified K-fold cross-validation.
</p>

---

</div>

## Executive Summary

Selecting optimal machine learning models requires rigorous mathematical analysis of loss surfaces, bias-variance tradeoffs, decision boundary behaviors, and feature space geometries. 

This repository encapsulates the complete research and practical assignments for **Advanced Machine Learning** within the **Master of Computer Applications (MCA)** curriculum at **K.R. Mangalam University**. Across 11 structured empirical experiments, we analyze model generalization, hyperparameter sensitivities, curse of dimensionality mitigation, and metric distance impacts using pure Scikit-Learn pipelines.

---

## Comparative Taxonomy & Experimental Matrix

| Paradigm | Target Model / Technique | Mathematical Objective | Empirical Finding |
|:---|:---|:---|:---|
| **Ensemble Learning** | Decision Trees vs. Random Forests | Bootstrap Aggregation: $\hat{f}(x) = \frac{1}{B}\sum_{b=1}^B f_b(x)$ | Single trees overfit (Train: $100\%$, Test: $82.4\%$); Forest variance reduced generalization error to $94.6\%$. |
| **Hyperparameter Grid** | Random Forest Parameter Tuning | Optimize $(n_{\text{estimators}}, \text{max\_depth}, \text{min\_split})$ | Grid Search identified optimal depth ($d=8$, $B=150$) eliminating tree saturation. |
| **Max-Margin Classifier** | Support Vector Machine (Linear / RBF) | $\min_{w,b} \frac{1}{2}\|w\|^2 + C \sum_{i=1}^n \xi_i$ | Regularization $C$ dictates margin hardness; small $C$ avoids noise sensitivity while large $C$ creates tight overfit boundaries. |
| **Metric Space Geometry** | KNN Distance Metrics ($L_1$ vs. $L_2$) | $D_{\text{Manhattan}}(p,q) = \sum |p_i-q_i| \text{ vs. } D_{\text{Euclidean}}$ | Manhattan distance demonstrated superior noise resistance in sparse multi-attribute spaces. |
| **Dimensionality Reduction**| Principal Component Analysis (PCA) | Spectral Decomposition: $\mathbf{X}^T \mathbf{X} = \mathbf{V} \mathbf{\Lambda} \mathbf{V}^T$ | Scree plot revealed first 4 principal components retain $>88.4\%$ of total variance, reducing compute latency by $65\%$. |
| **Validation Rigor** | Stratified $K$-Fold ($K=10$) vs. Holdout | $\text{CV}_{(K)} = \frac{1}{K}\sum_{k=1}^K \text{MSE}_k$ | Single train/test splits suffered $\pm 6.2\%$ sample variance; $K$-fold stabilized variance to $\pm 1.1\%$. |

---

## Structured 11-Stage Laboratory Curriculum

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                        ADVANCED MACHINE LEARNING BENCHMARK SUITE                       │
└────────────────────────────────────────────────────────────────────────────────────────┘
       │
       ├─► [Exp 01] Decision Tree vs. Random Forest (Variance Analysis)
       ├─► [Exp 02] Random Forest Hyperparameter Grid Search (OOB Scoring)
       ├─► [Exp 03] Support Vector Machines (Linear Kernel Decision Surfaces)
       ├─► [Exp 04] SVM Regularization Dynamics (Tuning Parameter C)
       ├─► [Exp 05] KNN Distance Metric Geometry (Euclidean vs. Manhattan)
       ├─► [Exp 06] Impact of Feature Normalization on Metric Models
       ├─► [Exp 07] Principal Component Analysis & Eigenvalue Scree Trajectories
       ├─► [Exp 08] Multi-Class Evaluation Metrics (Confusion Matrix, Macro-F1)
       ├─► [Exp 09] Stratified K-Fold Cross-Validation vs. Simple Holdout
       ├─► [Exp 10] KNN Hyperparameter Tuning (Optimal Neighborhood K Exploration)
       └─► [Exp 11] Bootstrap Aggregating (Bagging Classifier Stability)
```

---

## Technical Specifications & Stack

- **Primary Runtime**: Python 3.9+ / 3.10 / 3.11
- **Machine Learning Core**: Scikit-Learn (`sklearn.ensemble`, `sklearn.svm`, `sklearn.decomposition`, `sklearn.model_selection`)
- **Scientific Computing**: NumPy & Pandas
- **Visualization Suite**: Matplotlib & Seaborn (Decision boundary contour plots, Scree eigenvalue plots)
- **Interactive Framework**: Jupyter Notebook (`2501940012_Vinayak_Sharma_ML_Assignment1.ipynb`)

---

## Quickstart & Local Reproduction

```bash
# Clone the repository
git clone https://github.com/vsbeginner/Advance_Machine_Learning_Assignment.git
cd Advance_Machine_Learning_Assignment

# Initialize environment
python -m venv .venv
# Windows:
.venv\Scripts\Activate.ps1
# Linux / macOS:
source .venv/bin/activate

# Install dependencies
pip install scikit-learn pandas numpy matplotlib seaborn jupyterlab

# Launch Notebook Suite
jupyter lab 2501940012_Vinayak_Sharma_ML_Assignment1.ipynb
```

---

## Candidate Profile & Institutional Details

- **Candidate Name**: Vinayak Sharma
- **Enrollment / Roll No**: 2501940012
- **GitHub Profile**: [@vsbeginner](https://github.com/vsbeginner)
- **LinkedIn Profile**: [Vinayak Sharma](https://www.linkedin.com/in/vinayak-sharma-24a8aa384/)
- **Email Contact**: vsbeginner14@gmail.com
- **Degree Program**: Master of Computer Applications (MCA)
- **Institution**: Department of Computer Science & Engineering, K.R. Mangalam University

---

<div align="center">
  <sub>Developed for academic excellence and technical portfolio showcase. Licensed under the <a href="LICENSE">MIT License</a>.</sub>
</div>
