# CarPredict Analysis  

## Overview  
This repository contains the implementation and analysis of a **Car Price Prediction** project. The project aims to predict car prices using various data analysis, transformation, and machine learning techniques.  

---

## Libraries Used  
- **Numpy**: For numerical computations.  
- **Pandas**: For data manipulation and analysis.  
- **Matplotlib**: For data visualization.  
- **Scipy**: For statistical analysis.  
- **Seaborn**: For enhanced visualizations.  
- **Sklearn**: For building and evaluating machine learning models.  

---

## Workflow  

### 1. **Data Acquisition**  
- Data loaded into the `bpd` dataframe.  
- Column headers were added based on index numbers.  
- Dataset saved as CSV for future use.  

---

### 2. **Data Understanding**  
- Explored features and their data types.  
- Generated statistical summaries using `describe(include="all")`.  
- Used `info()` to inspect non-null values and data types.  

---

### 3. **Data Wrangling**  
Identified and handled missing data:  
1. **Identify missing data**.  
2. **Handle missing data**.  
3. **Correct data format**.  

---

### 4. **Data Transformation**  
- Converted quantitative features to appropriate metrics using mathematical techniques.  

---

### 5. **Data Normalization**  
- Normalized numerical features.  
- Used binning for categorizing numerical variables.  
- Applied **one-hot encoding** to convert categorical variables into numerical ones.  

---

### 6. **Exploratory Data Analysis (EDA)**  
- **Continuous Numerical Variables Analysis**: Regression plots to assess linear relationships.  
- **Categorical Variables Analysis**: Used box plots, `value_counts`, grouping, and pivot tables.  
- **Descriptive Statistical Analysis**: Heatmaps, correlation, causation, and ANOVA analysis.  

---

### 7. **Feature Selection**  
Key variables for price prediction:  
- **Continuous Numerical Variables**: Length, Width, Curb-weight, Engine-size, Horsepower, City-mpg, Highway-mpg, Wheel-base, Bore.  
- **Categorical Variables**: Drive-wheels.  

---

### 8. **Model Development**  
1. **Simple Linear Regression**: One independent variable.  
2. **Multiple Linear Regression (MLR)**: Multiple independent variables.  
3. **Polynomial Regression**: Non-linear relationships handled via polynomial transformations.  
4. **Pipelines**: Simplified data preprocessing and scaling using `Pipeline` and `StandardScaler`.  

---

### 9. **Model Evaluation**  
- Used regression and residual plots for model visualization.  
- Evaluated models using **R²** and **Mean Squared Error (MSE)** metrics.  

**Performance Metrics**:  
- **Simple Linear Regression**:  
  - R²: 0.6418  
  - MSE: 2.25 x 10⁷  
- **Multiple Linear Regression**:  
  - R²: 0.8119  
  - MSE: 1.2 x 10⁷  
- **Polynomial Regression**:  
  - R²: 0.6754  
  - MSE: 2.04 x 10⁷  

**Conclusion**: MLR provided the best results due to its ability to account for multiple variables.  

---

### 10. **Model Predictions**  
- Predicted outcomes for the test dataset using regression models.  
- Compared **training** and **testing** R² scores.  
- Applied `cross_val_score` to address limited test data issues.  

---

### 11. **Model Refinement**  
- **Techniques Used**:  
  - Polynomial Features  
  - Ridge Regression  
  - Hyperparameter Tuning (using `alpha` variable and Grid Search).  

- **Optimized Result**: Achieved an R² score of **0.84** for the test dataset after optimization.  

---

## Key Insights  
Through the systematic application of machine learning models and evaluation techniques, we identified that the **Multiple Linear Regression model** offers the best predictive power for car price estimation. The use of model refinement and hyperparameter tuning further improved prediction accuracy.  

---  

## Repository Structure  
- **auto.csv/**: Contains raw and processed datasets.  
- **OLD CAR PRICE DATASET ANALYSIS/**: Jupyter notebooks with detailed analysis and visualization on dataset.
- **MODEL DEVELOPMENT AND EVALUATION/**: Jupyter notebooks with detailed model development, analysis, visualization, and refinement on dataset.

---

## Conclusion  
This project provides a robust framework for car price prediction using exploratory data analysis and machine learning techniques. The repository can be extended for other regression problems with similar workflows.  

For contributions or feedback, feel free to raise an issue or submit a pull request! 🚗📊
