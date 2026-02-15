# heart_disease_full_pipeline
**Goal:** Predict heart disease presence using clinical data from the UCI dataset.

---

## 🚀 Summary
Built a full ML classification pipeline for medical diagnosis.
- Models trained: Logistic Regression, Random Forest, Gradient Boosting.
- Best model: Random Forest (AUC = 0.98, Recall = 0.90)
- Emphasized recall to reduce false negatives (critical in medical screening).

---

## 📊 Results
| Model | ROC AUC | F1 | Recall |
|--------|----------|------|--------|
| Logistic Regression | 0.96 | 0.88 | 0.86 |
| Random Forest | **0.98** | **0.91** | **0.90** |
| Gradient Boosting | 0.97 | 0.89 | 0.88 |

---

## 🧠 Insights
- **Most important features:** `cp` (chest pain type), `thalach` (max heart rate), `oldpeak`, and `ca`.
- **Interpretation:** Higher chest pain frequency, lower exercise tolerance, and higher ST depression correlate with heart disease risk.

---

## 🧾 How to Run
```bash
pip install numpy pandas scikit-learn seaborn matplotlib shap joblib
python heart_disease_full_pipeline.ipynb
