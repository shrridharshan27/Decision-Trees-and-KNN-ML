# ML Lab 04: Decision Trees & K-Nearest Neighbors (KNN)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-013243.svg?logo=numpy&logoColor=white)](https://numpy.org/)

---

## Academic Details
- **Student Name:** Shrri Dharshan D R
- **Register Number:** 23BPS1090
- **Course Code:** BCSE209P
- **Course Title:** Machine Learning Laboratory
- **Faculty:** Dr. S. Shridevi
- **Institution:** School of Computer Science and Engineering (SCOPE), VIT Chennai

---

## Overview
This repository contains laboratory implementations and empirical comparative evaluations of **Decision Tree Classifiers** and **K-Nearest Neighbors (KNN)** algorithms across binary and multi-class classification benchmark problems from the UCI Machine Learning Repository.

The laboratory examines recursive binary partitioning, splitting criteria (Gini Impurity vs. Information Gain / Entropy), tree pruning strategies, and instance-based non-parametric learning via distance metrics (Euclidean, Manhattan), feature scaling sensitivity, and hyperparameter optimization ($k$-selection).

---

## Experiments & Datasets

### 1. Decision Tree — Bank Marketing Term Deposit Subscription
- **Dataset:** Bank Marketing Dataset ([UCI ID: 222](https://archive.ics.uci.edu/dataset/222))
- **Objective:** Predict whether a client will subscribe to a term deposit (`yes` / `no`).
- **Notebook:** [23BPS1090_ShrriDharshan_ML_Lab_DT_BankMarketing.ipynb](./23BPS1090_ShrriDharshan_ML_Lab_DT_BankMarketing.ipynb)
- **Techniques:** Splitting criterion comparison (Gini vs. Entropy), max-depth pruning, feature importance extraction, and decision tree visualization.

### 2. Decision Tree — Dry Bean Multi-Class Variety Classification
- **Dataset:** Dry Bean Dataset ([UCI ID: 602](https://archive.ics.uci.edu/dataset/602))
- **Objective:** Classify dry bean grains into 7 registered varieties (Seker, Barbunya, Bombay, Cali, Dermosan, Horoz, Sira) using 16 morphological and shape features.
- **Notebook:** [23BPS1090_ShrriDharshan_ML_Lab_DT_DryBean.ipynb](./23BPS1090_ShrriDharshan_ML_Lab_DT_DryBean.ipynb)
- **Techniques:** Multi-class classification, tree depth regularization, and pruning analysis.

### 3. K-Nearest Neighbors (KNN) — Bank Marketing
- **Dataset:** Bank Marketing Dataset ([UCI ID: 222](https://archive.ics.uci.edu/dataset/222))
- **Objective:** Predict client term deposit subscription using instance-based neighborhood voting.
- **Notebook:** [23BPS1090_ShrriDharshan_ML_Lab_KNN_BankMarketing.ipynb](./23BPS1090_ShrriDharshan_ML_Lab_KNN_BankMarketing.ipynb)
- **Techniques:** Standard scaling, parameter search for optimal neighbor count ($k$), uniform vs. distance-weighted voting.

### 4. K-Nearest Neighbors (KNN) — Dry Bean Multi-Class Classification
- **Dataset:** Dry Bean Dataset ([UCI ID: 602](https://archive.ics.uci.edu/dataset/602))
- **Objective:** Multi-class classification of dry bean varieties based on morphological distances.
- **Notebook:** [23BPS1090_ShrriDharshan_ML_Lab_KNN_DryBean.ipynb](./23BPS1090_ShrriDharshan_ML_Lab_KNN_DryBean.ipynb)
- **Techniques:** High-dimensional distance computations, metric comparison (Euclidean vs. Manhattan), and $k$-fold cross-validation.

---

## Evaluation Metrics
- **Classification Accuracy & Balanced Accuracy**
- **Precision, Recall, and F1-Score** (Macro, Micro, and Weighted)
- **Confusion Matrices** with class error heatmaps
- **Receiver Operating Characteristic (ROC-AUC)**
- **Complexity Curves:** Training vs. validation error across varying tree depths and $k$-values

---

## Repository Structure
```text
ML-Lab-04-Decision-Trees-and-KNN/
├── 23BPS1090_ShrriDharshan_ML_Lab_DT_BankMarketing.ipynb
├── 23BPS1090_ShrriDharshan_ML_Lab_DT_DryBean.ipynb
├── 23BPS1090_ShrriDharshan_ML_Lab_KNN_BankMarketing.ipynb
├── 23BPS1090_ShrriDharshan_ML_Lab_KNN_DryBean.ipynb
├── bank_marketing_data/
├── .gitignore
└── README.md
```

---

## How to Run
1. **Clone the repository:**
   ```bash
   git clone https://github.com/shrridharshan27/ML-Lab-04-Decision-Trees-and-KNN.git
   cd ML-Lab-04-Decision-Trees-and-KNN
   ```
2. **Install dependencies:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn ucimlrepo jupyter
   ```
3. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```
