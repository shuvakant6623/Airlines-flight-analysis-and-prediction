# ✈ Airline Flights Data Analysis & Modeling

## 📌 Overview
This project performs **Exploratory Data Analysis (EDA)**, **statistical tests**, **data preprocessing**, and **machine learning modeling** on an airline flights dataset.

The workflow includes:
- Data inspection
- Descriptive statistics
- Outlier detection & visualization
- Categorical frequency and association analysis
- ANOVA tests
- Data preprocessing (winsorization & label encoding)
- Model training & evaluation

---

## 📂 Dataset
**File:** `airlines_flights_data.csv`  
**Type:** Tabular  
**Content:** Flight details such as airline, source/destination cities, duration, price, stops, class, and more.

---

## 🔍 Steps & Functions

### **1. Data Exploration**
- Display **head**, **tail**, **info**, and **describe**.
- Sampling & shape inspection.

### **2. Descriptive Statistics**
Function: `descriptive_analysis()`  
- Computes statistical measures (mean, median, std, percentiles, skew, kurtosis).
- Detects outliers using **IQR method**.

### **3. Distribution & Outlier Visualization**
Function: `plot_numerical_distribution()`  
- Histograms & KDE plots.
- Boxplots for outlier visualization.

### **4. Correlation Analysis**
Function: `plot_correlation_matrix()`  
- Computes **Spearman correlation** for numeric features.
- Heatmap visualization.

### **5. Frequency Analysis**
Function: `Freq_analysis()`  
- Plots top N categories for each categorical variable.

### **6. Cardinality & Rare Categories**
Function: `analyze_cardinality()`  
- Identifies rare categories (below a set frequency threshold).
- Suggests dropping or binning rare categories.

### **7. Categorical Associations**
Function: `chi_square_test()`  
- Performs Chi-Square test between categorical variables.
- Calculates **Cramer's V** to determine strength of association.

### **8. Grouped Statistics**
Function: `plot_grouped_stats()`  
- Mean, median, std, and count of numeric variables grouped by categories.
- Barplot visualizations.

### **9. ANOVA Tests**
Function: `anova_test()`  
- Tests statistical differences in numeric features across categories.

### **10. Data Preprocessing**
- **Winsorization:** Removes extreme outliers (`Winsorization_col()`).
- **Label Encoding:** Encodes categorical variables numerically (`label_encoding()`).

### **11. Model Selection**
Class: `ModelSelection`  
Models tested:
- KNN  
- Logistic Regression  
- Decision Tree  
- Random Forest  
- (CatBoost and SVM initialized but not evaluated in summary table)

Outputs a dataframe with train/test scores.

### **12. Cross-Validation**
- Performs **5-fold cross-validation** for Decision Tree & Random Forest.
- Displays individual fold accuracies and mean accuracy.

---


