# 🎬 Movie Revenue & Success Prediction

This project aims to predict the **revenue** and **success status** of movies based on pre-release metadata such as genres, budget, language, popularity, etc. The dataset is derived from [TMDb (The Movie Database)](https://www.themoviedb.org/).

---

## 🔍 Objectives

- 🧮 Predict **total revenue** (regression)
- ✅ Predict whether a movie will be **successful** or not (classification)

---

## 📦 Features Used

- Budget, genres, language
- Popularity, release date
- Runtime, vote average/count
- Overview embeddings (TF-IDF vectors)

---

## ⚙️ Models Used

- **Logistic Regression** for classification
- **Random Forest Regressor** for revenue prediction

All models were trained with `Pipeline` and hyperparameters tuned using `GridSearchCV`.

---

## 📊 Performance

### 📈 Classification
- Accuracy: **0.72**
- ROC AUC: **0.78**

### 💰 Regression
- R² Score: **0.78**
- RMSE: **$75.9M**

---

## 🖼️ Visualizations

All model evaluation plots are saved under `images/`:
- Confusion Matrix
- ROC Curve
- Actual vs Predicted Revenue
- Residual Plot

---

## 🧪 Notebooks

- `01_eda.ipynb`: Data cleaning and exploration
- `02_modeling.ipynb`: Feature engineering, training, and tuning
- `03_evaluation.ipynb`: Visual model evaluation

---

## 💾 Installation

```bash
pip install -r requirements.txt
```

---

## ✅ Conclusion

The models demonstrate solid predictive power, especially in identifying successful movies. Future improvements may include ensemble methods or deep learning for more robust results.