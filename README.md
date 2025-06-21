# 🦴 Predicting Osteoporosis Risk

## 📌 Project Overview

This project aims to develop a **machine learning model** that predicts the **risk of osteoporosis** in patients using a variety of **demographic, medical, lifestyle, and nutritional factors**. The model is designed to support early diagnosis, personalized treatment planning, and efficient healthcare resource allocation.

---

## 🧪 Dataset Description

* **Rows**: 1,958 patient records
* **Target Variable**: `Osteoporosis` (Binary: 0 = No, 1 = Yes)
* **Key Features**:

  * Age
  * Gender
  * Hormonal Changes
  * Family History
  * Race/Ethnicity
  * Body Weight
  * Calcium & Vitamin D Intake
  * Physical Activity
  * Smoking & Alcohol Consumption
  * Medical Conditions & Medications
  * Prior Fractures

> Missing values were handled by **dropping incomplete rows** for this version of the model.

---

## 🛠 Tools & Technologies

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Jupyter Notebook

---

## 🔄 Data Preprocessing

* Dropped rows with missing values using `df.dropna()`
* Label encoded categorical variables
* Removed the `Id` column
* Split data into **training and test sets (80/20)**

---

## 📊 Exploratory Data Analysis (EDA)

* Count plots for **Calcium** and **Vitamin D** intake vs Osteoporosis
* Correlation heatmap for numerical features

---

## 🤖 Model Training & Evaluation

Tested four classification models:

1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest** ✅ *(Best Performing Model)*
4. **Support Vector Machine (SVM)**

**Best Model**: **Random Forest Classifier**

* Tuned using **GridSearchCV**
* Evaluated using:

  * Accuracy
  * Precision
  * Recall
  * F1-Score
  * ROC Curve and AUC Score

---

## 💡 Key Insights

* Patients with **low calcium and vitamin D intake** show a higher risk of osteoporosis.
* **Hormonal changes**, **prior fractures**, and **existing medical conditions** are strong predictors.
* Random Forest offered the best balance of **performance and interpretability**.

---

## 📁 Project Structure

```bash
.
├── Predicting_Osteoporosis_Risk.ipynb   # Main notebook
├── osteoporosis_dataset.csv             # Dataset
└── README.md                            # Project summary
```

---

## ▶️ How to Run

1. **Install dependencies:**

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

2. **Launch Jupyter Notebook:**

   ```bash
   jupyter notebook
   ```

3. **Open and run:** `Predicting_Osteoporosis_Risk.ipynb`

---

## 👨‍💻 Author

**Pratik Bokade**
🔗 [LinkedIn](https://www.linkedin.com/in/ask-pratik-bokade)
