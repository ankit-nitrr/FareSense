# ✈️ FareSense - Airfare Forecasting System

A machine learning project to predict flight ticket prices based on features such as airline, duration, class, departure time, and more.

---

## 🔍 Objective

To develop regression models that accurately predict flight prices using exploratory data analysis, preprocessing pipelines, and ensemble learning techniques.

---

## 📂 Project Structure

- **EDA & Cleaning**: Missing values, duplicates, and outliers explored and handled. Categorical and numerical features analyzed.
- **Preprocessing**: Feature engineering (frequency encoding for the high-cardinality `flight` column), custom pipelines for imputation, encoding, and scaling.
- **Modeling**: Trained and tuned 3 regression models — Linear Regression, Random Forest, and XGBoost.
- **Evaluation**: Assessed using R², RMSE, and MAE on validation and test sets.

---

## 🧰 Tech Stack

- **Language**: Python
- **Libraries**: pandas, numpy, scikit-learn, XGBoost, matplotlib, seaborn, scipy
- **Tools**: Jupyter Notebook, GitHub

---

## 📊 Key Highlights

- ✨ EDA revealed insightful trends: price vs. duration (positive), price vs. days_left (negative).
- 🔁 Applied log transformation to stabilize skewed price distribution.
- 🔧 Tuned hyperparameters using `RandomizedSearchCV` on the tree-based models.
- 🛠️ Used column-wise transformers with Pipelines for clean, reproducible preprocessing.
- 🏆 Selected the best model based on validation R² and retrained it on the full training set before testing.

---

## 📈 Final Results

| Model              | R² Score |   RMSE      |   MAE      |
|--------------------|----------|-------------|------------|
| XGBoost            |   0.98   |  3162.50    |  1696.73   |
| Random Forest      |   0.98   |  3536.20    |  1909.01   |
| Linear Regression  |   0.88   |  7946.11    |  4653.12   |

---

## 🧠 ML Models Used

- Linear Regression
- Random Forest Regressor
- XGBoost Regressor

---

## 🚀 How to Run

```bash
git clone <your-repo-url>
cd airfare-forecasting-system
pip install -r requirements.txt
jupyter notebook airfare-forecasting-system.ipynb
```

---

## 📬 Contact

For queries, feel free to reach out via GitHub.
