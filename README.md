# 🚗 CarPredict: Advanced Car Price Estimation  

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.2%2B-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)

An end-to-end Machine Learning project focused on predicting automobile prices using a comprehensive dataset of car characteristics. This project demonstrates a complete data science lifecycle, from raw data acquisition to a high-performing predictive model.

---

## 🎯 Project Objective
The goal is to develop an accurate estimation model for used car prices based on features like engine size, horsepower, curb weight, and fuel efficiency. This assists both buyers and sellers in determining fair market value.

**Key Achievement:** Developed a refined model achieving an **R² score of 0.84**, significantly improving upon baseline linear regression models.

---

## 🛠️ Tech Stack & Skills
- **Data Manipulation**: `Pandas`, `NumPy`
- **Visualization**: `Matplotlib`, `Seaborn` (Regression plots, box plots, heatmaps)
- **Mathematical Modeling**: `Scipy`
- **Machine Learning**: `Scikit-Learn` (Linear Regression, Polynomial Regression, Ridge Regression, Grid Search)
- **Preprocessing**: `StandardScaler`, `LabelEncoder`, `One-Hot Encoding`

---

## 🚀 Project Workflow

### 1. Data Wrangling & Cleaning
- Handled missing values (symbolized by '?') through mean imputation and frequency substitution.
- Corrected data formats for numerical features.
- Normalized quantitative features to ensure uniform scaling.

### 2. Exploratory Data Analysis (EDA)
- Analyzed **Continuous Variables** using regression plots to visualize linear relationships with price.
- Analyzed **Categorical Variables** using box plots to evaluate their predictive power.
- Conducted **Pearson Correlation** and **ANOVA** to identify critical features.

### 3. Model Development
Iteratively built and evaluated multiple regression architectures:
- **Simple Linear Regression (SLR)**: Baseline model.
- **Multiple Linear Regression (MLR)**: Incorporated multiple influential features.
- **Polynomial Regression**: Captured non-linear trends.
- **Data Pipelines**: Streamlined scaling and transformations.

### 4. Model Evaluation & Refinement
- Utilized **Cross-Validation** to ensure model generalizability.
- Performed **Ridge Regression** to mitigate overfitting.
- Optimized hyperparameters using **Grid Search** (tuning `alpha` for Ridge).

---

## 📊 Performance Summary

| Model Type                 | R² Score | Mean Squared Error (MSE) |
|----------------------------|----------|--------------------------|
| Simple Linear Regression   | 0.6418   | 2.25 x 10⁷               |
| Polynomial Regression      | 0.6754   | 2.04 x 10⁷               |
| Multiple Linear Regression | 0.8119   | 1.20 x 10⁷               |
| **Refined Ridge Model**    | **0.8400** | *Optimized*              |

---

## 📁 Repository Structure
```text
├── OLD CAR PRICE DATASET ANALYSIS.ipynb      # Detailed Data Wrangling & EDA
├── MODEL DEVELOPMENT AND EVALUATION.ipynb    # Model Building & Hyperparameter Tuning
├── auto.csv                                  # Raw Dataset
├── subsimple/                                # Compressed project files
└── README.md                                 # Project Documentation
```

---

## 📥 Installation & Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/ANKIT21111/CarPredict.git
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn scipy
   ```
3. Run the Jupyter Notebooks:
   ```bash
   jupyter notebook
   ```

---

## 💡 Key Insights
- **Engine Size**, **Curb Weight**, and **Horsepower** emerged as the strongest predictors of car price.
- Non-linear relationships were successfully captured using Polynomial transformations, but **Multiple Linear Regression** provided the best balance of complexity and accuracy.
- Hyperparameter tuning through Ridge Regression was essential in reducing variance and achieving the final R² of 0.84.

---

## 👨‍💻 Author
**Ankit Abhishek**  
Data Engineering Professional | Machine Learning Enthusiast  
[LinkedIn](https://www.linkedin.com/in/ankitabhishekdataengineering/) | [Portfolio](https://ankitabhishek.com)

---
*If you find this project useful, feel free to ⭐ the repository!*
