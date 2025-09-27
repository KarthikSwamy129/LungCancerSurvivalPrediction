# 🫁 Lung-Cancer-Survival-Prediction

A tiny end-to-end machine-learning project that predicts whether a lung-cancer patient will survive based on diagnosis data.

---

## 📦 What's inside
| File | Purpose |
|------|---------|
| `dataset_med.csv` | 1 700+ patient records (features + survival flag) |
| `lung_cancer_survival_model.pkl` | Trained scikit-learn Random-Forest model |
| 'Detect Lung Cancer using patient diagnosis data' | About Project |
| `LungCancerSurvival.ipynb` | Google-Colab notebook that builds & evaluates the model |

---

## 🚀 Quick start (Google Colab)
1. Open [`train.ipynb`](https://colab.research.google.com/github/YOUR_USER/YOUR_REPO/blob/main/train.ipynb)  
2. Runtime → Run all  
3. Download `lung_cancer_survival_model.pkl` and place it in the same notebook.
Follow the prompts → get instant survival prediction (0 = no, 1 = yes).


📊 Model snapshot
Algorithm: Random-ForestClassifier (50 trees, max_depth 10)
Accuracy on hold-out set: ~85 %
Input: 13 features (age, BMI, stage, smoking status, treatment, etc.)
Output: binary survival flag + probability


📝 Notes
All categorical columns are label-encoded inside the scripts – no extra preprocessing needed.
Dataset is synthetic / anonymised; no PHI or HIPAA concerns.
Feel free to swap in XGBoost, logistic regression, or neural nets.
