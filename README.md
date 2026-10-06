# Decision Trees & K-Nearest Neighbors (KNN)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-013243.svg?logo=numpy&logoColor=white)](https://numpy.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Author
- **Shrri Dharshan D R** — [@shrridharshan27](https://github.com/shrridharshan27)

---

## Overview
This repository implements and benchmarks **Decision Tree Classifiers** (parametric tree-based recursive partitioning) and **K-Nearest Neighbors (KNN)** (instance-based non-parametric learning) across binary and multi-class classification benchmark tasks from the UCI Machine Learning Repository.

The project evaluates splitting criteria (Gini Impurity vs. Information Gain / Entropy), tree depth constraints, pruning regularization, distance metrics (Euclidean, Manhattan), feature normalization effects, and optimal neighbor count selection ($k$).

---

## Project Modules & Datasets

### 1. Decision Trees — Bank Marketing Term Deposit Subscription
- **Dataset:** Bank Marketing Dataset ([UCI ID: 222](https://archive.ics.uci.edu/dataset/222))
- **Objective:** Predict client term deposit subscription (`yes` / `no`).
- **Notebook:** [`23BPS1090_ShrriDharshan_ML_Lab_DT_BankMarketing.ipynb`](./23BPS1090_ShrriDharshan_ML_Lab_DT_BankMarketing.ipynb)
- **Methodology:** Criterion comparison (Gini vs. Entropy), max-depth hyperparameter pruning, and feature importance rankings.

### 2. Decision Trees — Dry Bean Multi-Class Variety Classification
- **Dataset:** Dry Bean Dataset ([UCI ID: 602](https://archive.ics.uci.edu/dataset/602))
- **Objective:** Classify dry beans into 7 registered commercial varieties using 16 computer vision geometric shape features.
- **Notebook:** [`23BPS1090_ShrriDharshan_ML_Lab_DT_DryBean.ipynb`](./23BPS1090_ShrriDharshan_ML_Lab_DT_DryBean.ipynb)
- **Methodology:** Multi-class tree recursive splitting and complexity pruning.

### 3. K-Nearest Neighbors (KNN) — Bank Marketing
- **Dataset:** Bank Marketing Dataset ([UCI ID: 222](https://archive.ics.uci.edu/dataset/222))
- **Objective:** Instance-based customer conversion prediction.
- **Notebook:** [`23BPS1090_ShrriDharshan_ML_Lab_KNN_BankMarketing.ipynb`](./23BPS1090_ShrriDharshan_ML_Lab_KNN_BankMarketing.ipynb)
- **Methodology:** Standard feature scaling, optimal $k$ search, uniform vs. distance-weighted voting.

### 4. K-Nearest Neighbors (KNN) — Dry Bean Multi-Class Classification
- **Dataset:** Dry Bean Dataset ([UCI ID: 602](https://archive.ics.uci.edu/dataset/602))
- **Objective:** Morphological multi-class variety classification.
- **Notebook:** [`23BPS1090_ShrriDharshan_ML_Lab_KNN_DryBean.ipynb`](./23BPS1090_ShrriDharshan_ML_Lab_KNN_DryBean.ipynb)
- **Methodology:** Distance metric evaluation (Euclidean vs. Manhattan) and cross-validated error analysis.

---

## Evaluation Metrics
- **Accuracy & Balanced Accuracy**
- **Precision, Recall, and F1-Score** (Macro and Weighted)
- **Multi-Class Confusion Matrices**
- **Model Complexity Curves:** Tracking training vs. test error over tree depth and $k$-values

---

## Project Structure
```text
Decision-Trees-and-KNN-ML/
├── 23BPS1090_ShrriDharshan_ML_Lab_DT_BankMarketing.ipynb
├── 23BPS1090_ShrriDharshan_ML_Lab_DT_DryBean.ipynb
├── 23BPS1090_ShrriDharshan_ML_Lab_KNN_BankMarketing.ipynb
├── 23BPS1090_ShrriDharshan_ML_Lab_KNN_DryBean.ipynb
├── bank_marketing_data/
├── .gitignore
└── README.md
```

---

## Quickstart & Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/shrridharshan27/Decision-Trees-and-KNN-ML.git
   cd Decision-Trees-and-KNN-ML
   ```
2. **Install requirements:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn ucimlrepo jupyter
   ```
3. **Run the notebooks:**
   ```bash
   jupyter notebook
   ```

---

## License
Distributed under the [MIT License](https://opensource.org/licenses/MIT).
