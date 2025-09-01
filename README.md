# 🏥 Medical Insurance Cost Prediction

## 📌 Project Overview

This project predicts **medical insurance costs** of individuals based on features such as **age, BMI, smoking habits, gender, and region**.
We compare **Linear Regression** (simple & interpretable) vs **Random Forest Regressor** (powerful & flexible).

---

## 📂 Dataset

* Source: [Kaggle - Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)
* Columns:

  * `age`: Age of the primary beneficiary
  * `sex`: Gender (male/female)
  * `bmi`: Body mass index (weight/height²)
  * `children`: Number of children covered by insurance
  * `smoker`: Smoking status (yes/no)
  * `region`: Residential area (northeast, northwest, southeast, southwest)
  * `charges`: Insurance cost (target variable)

---

## ⚙️ Project Workflow

1. **Load Libraries** – Import required Python packages
2. **Load Dataset** – Read CSV file and view structure
3. **EDA (Exploratory Data Analysis)**

   * Summary statistics
   * Correlation analysis
   * Visualization with Seaborn/Matplotlib
4. **Data Preprocessing**

   * Encode categorical variables (`sex`, `smoker`, `region`)
   * Train/Test split
   * Scaling features (for linear regression)
5. **Model Training**

   * Linear Regression
   * Random Forest Regressor
6. **Model Evaluation**

   * Metrics: `R²`, `RMSE`
   * Feature Importance (for Random Forest)
7. **Model Comparison**

---

## 📊 Results

| Model             | R² Score | RMSE   |
| ----------------- | -------- | ------ |
| Linear Regression | \~0.74   | \~6000 |
| Random Forest     | \~0.85   | \~4500 |

👉 **Random Forest outperforms Linear Regression**, especially in capturing non-linear relationships (e.g., smokers dramatically increasing charges).

---

## 🚀 Tech Stack

* **Python**
* **Pandas, NumPy** – Data manipulation
* **Matplotlib, Seaborn** – Visualization
* **Scikit-learn** – ML models & preprocessing

---

## 💡 Key Insights

* **Smoking** is the most important factor affecting insurance cost.
* **BMI** and **Age** also strongly influence charges.
* Random Forest captures these complex interactions better than Linear Regression.

---

## 📌 Future Improvements

* Hyperparameter tuning with `GridSearchCV`
* Try advanced models like **XGBoost**
* Build a **web app (Streamlit/Flask)** for user input → insurance cost prediction

---

## 📁 Repository Structure

```
📦 Medical-Insurance-Cost-Prediction
 ┣ 📜 insurance.csv          # Dataset
 ┣ 📜 medical_insurance.ipynb # Jupyter/Colab Notebook
 ┣ 📜 README.md               # Project Documentation
 ┗ 📜 requirements.txt        # Dependencies
```

