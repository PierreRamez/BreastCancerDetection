# 🎗️ Breast Cancer Detection

A fun, semi-formal demo of a Logistic Regression–based classifier to distinguish benign vs. malignant tumors using the Wisconsin dataset. Perfect as a portfolio piece—complete with EDA, preprocessing, modeling, and evaluation.

---

## 🚀 Features

- **Exploratory Data Analysis**: Seaborn visualizations of feature distributions, correlations, and class balance  
- **Preprocessing Pipeline**:  
  - Dropped irrelevant columns (`id`, low‑variance features)  
  - Scaled features to zero mean & unit variance  
- **Modeling**:  
  - Logistic Regression classifier  
  - Reproducible train/test split (random seed)  
- **Evaluation**:  
  - Confusion matrix  
  - Precision, recall, F1-score  
  - ROC curve & AUC

---



## ⚙️ Installation

1. Clone the repo:  
   ```bash
   git clone https://github.com/your-username/BreastCancerDetection.git
   cd BreastCancerDetection
  

2. Create & activate a virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate      # on Windows: venv\Scripts\activate
   ```
---

## 🚴‍♀️ Quickstart

1. **Train the model**

   ```bash
   python src/train.py --data-path data/data.csv --output-dir outputs
   ```
2. **Evaluate & plot**

   ```bash
   python src/evaluate.py --model-path outputs/logreg.pkl --data-path data/data.csv --output-dir outputs
   ```
3. **Check outputs**

   * `outputs/confusion_matrix.png`
   * `outputs/roc_curve.png`

---

## 📈 Performance

| Metric    | Score |
| --------- | ----: |
| Accuracy  | 95.6% |
| Precision |  0.96 |
| Recall    |  0.95 |
| F1-Score  |  0.95 |
| AUC       |  0.98 |

---

## 🛠️ Contributing

PRs & issues welcome! Ideas:

* Hyperparameter tuning (GridSearchCV, RandomizedSearchCV)
* Alternative models (XGBoost, SVM)
* Dockerization & CI/CD pipeline

---

## 📜 License

MIT © 2025 Pierre Ramez Francis

---

Made with ☕ & 🤖 — because AI + coffee = magic!

