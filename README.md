# Employee-Salary-Prediction-using-Xgboost-

This project aims to predict employee salary class (`<=50K` or `>50K`) using various machine learning models. The dataset is based on demographic, educational, and employment-related attributes. Multiple models were tested and evaluated to determine the most accurate predictor.

## 📁 Dataset

- **Name**: [Adult Census Income Dataset]
- **Source**: UCI Machine Learning Repository
- **Path Used in Code**: `/content/drive/MyDrive/adult 3.csv`

The dataset contains information like age, work class, education, marital status, occupation, etc., and the target is to predict whether the income is greater than $50K or not.

---

## 🚀 Technologies Used

- Python
- Google Colab
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

---

## 🧪 Models Used

| Model               | Accuracy | Log Loss |
|--------------------|----------|----------|
| Logistic Regression| ✔️       | ✔️       |
| Decision Tree      | ✔️       | ✔️       |
| Random Forest      | ✔️       | ✔️       |
| Support Vector Machine (SVM) | ✔️ | ✔️ |
| **XGBoost (Final Model)** | **✅ Highest** | ✅ Lowest |

The final XGBoost model achieved the best performance and is visualized through accuracy and log-loss graphs across 100 boosting rounds.

---

## 📊 Visualizations

- Comparison bar charts of **Accuracy** and **Log Loss** for all models.
- Line plots showing **XGBoost accuracy** and **log loss** over 100 boosting rounds.

---

## 🧹 Data Preprocessing

- Missing values handled by replacing `' ?'` with `NaN` and dropping missing rows.
- Categorical columns encoded using `LabelEncoder`.
- Features normalized using `StandardScaler`.

---

## 🧠 Model Evaluation

- Train-Test Split: 80/20
- Metrics:
  - Accuracy Score
  - Log Loss
- Final predictions made using a threshold of 0.5 for XGBoost.

---

## 📈 Final Results (XGBoost)

- **Accuracy**: ~`0.87`
- **Log Loss**: ~`0.31`

---

## 📌 How to Run

1. Upload the dataset (`adult 3.csv`) to your Google Drive.
2. Open the provided Colab notebook.
3. Ensure required libraries are installed:
   ```bash
   pip install xgboost
   ```
4. Run all cells to train and evaluate models.

---

## 📚 Future Improvements

- Hyperparameter tuning using GridSearchCV.
- Deploy the model using Flask or Streamlit.
- Explore feature importance with SHAP values.

---

