# 🎗️ Breast Cancer Detection

A practical demo of breast cancer classification using the Wisconsin dataset.  
Now extended beyond Logistic Regression to include **SVM** and **XGBoost**, with improved evaluation and validation.  
Perfect as a portfolio piece—complete with EDA, preprocessing, modeling, benchmarking, and metrics.

---

## 🚀 Features

- **Exploratory Data Analysis**: Seaborn visualizations of feature distributions, correlations, and class balance  
- **Preprocessing**:  
  - Dropped irrelevant columns (`id`, low-variance features)  
  - Proper train/test split before scaling (fixes potential data leakage)  
- **Modeling**:  
  - Logistic Regression  
  - Support Vector Machine (SVM)  
  - XGBoost  
- **Evaluation**:  
  - Confusion matrix  
  - Precision, recall, F1-score  
  - ROC curve & AUC  
  - Cross-validation with stratification for reliable estimates  
  - Training vs. inference time benchmarking  

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

| Model               |  F1-Score | ROC-AUC | Notes                        |
| ------------------- | --------: | ------: | ---------------------------- |
| Logistic Regression | **0.976** |   0.99+ | Strong baseline, very fast   |
| SVM                 |     0.961 |   0.99+ | Competitive, efficient train |
| XGBoost             |     0.953 |   0.99+ | Slightly lower, tunable      |


---

## 🛠️ Contributing

PRs & issues welcome! Ideas:

* Hyperparameter tuning (GridSearchCV, RandomizedSearchCV)
* Dockerization & CI/CD pipeline
* Feature engineering & dimensionality reduction
* Deployment (Flask, Docker, or Streamlit app)

---

## 📜 License

MIT © 2025 Pierre Ramez Francis

---

Made with ☕ & 🤖 — because AI + coffee = magic!

