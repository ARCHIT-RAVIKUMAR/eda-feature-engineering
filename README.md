# Used Car Price Prediction - Exploratory Data Analysis, Data Cleaning & Feature Engineering

## 📌 Project Overview

This project performs Exploratory Data Analysis (EDA), Data Cleaning, and Feature Engineering on the **Used Car Price Prediction** dataset. The objective is to understand the dataset, identify data quality issues, prepare the data for machine learning, and create meaningful features that can improve the performance of future predictive models.

---

# 📂 Dataset Overview

The dataset contains information about used cars listed for sale, including details such as:

* Brand
* Model
* Model Year
* Mileage
* Fuel Type
* Engine
* Transmission
* Exterior Color
* Interior Color
* Accident History
* Clean Title Status
* Price

The primary objective of this dataset is to predict the selling price of a used car based on its characteristics.

---

# 🔍 Data Quality Issues Identified

During the exploratory analysis, the following data quality issues were observed:

* Missing values were present in multiple columns.
* Duplicate records existed in the dataset.
* The **milage** column was stored as text (e.g., `51,000 mi.`) instead of numeric values.
* Numerical and categorical features required different preprocessing techniques.
* Some numerical columns contained potential outliers.

---

# 🧹 Data Cleaning Techniques Applied

The following preprocessing steps were performed:

* Filled missing numerical values using the **median**.
* Filled missing categorical values using the **mode**.
* Removed duplicate records.
* Converted the **milage** column from text to numeric format.
* Verified that no missing values or duplicate records remained after cleaning.

---

# ⚙️ Feature Engineering

Five meaningful features were created to improve future machine learning models:

1. **Car_Age** – Calculates the age of the vehicle.
2. **Mileage_Per_Year** – Average distance driven per year.
3. **Is_Luxury_Brand** – Indicates whether the vehicle belongs to a luxury brand.
4. **High_Mileage** – Identifies vehicles with mileage above the dataset median.
5. **High_Performance** – Flags vehicles equipped with V8, V10, or V12 engines.

These engineered features provide additional information that can improve price prediction accuracy.

---

# 📊 Exploratory Data Analysis Performed

The notebook includes:

* Dataset overview
* Dataset shape
* Data types
* Summary statistics
* Missing value analysis
* Duplicate record analysis
* Numerical and categorical feature identification
* Unique value analysis
* Distribution of categorical features
* Outlier detection
* Data cleaning
* Feature engineering

---

# 💡 Key Insights

1. The dataset contains a combination of numerical and categorical features that require preprocessing before machine learning.
2. Missing values and duplicate records were successfully handled, improving overall data quality.
3. Converting mileage from text to numeric format enabled meaningful calculations and feature engineering.
4. Engineered features such as Car Age, Mileage Per Year, Luxury Brand Indicator, High Mileage Indicator, and High Performance Engine can provide valuable information for predicting vehicle prices.
5. The cleaned dataset is well-prepared for future regression models aimed at predicting used car prices.

---

# 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook

---

# 📁 Repository Structure

```text
epochs26-day03-eda-feature-engineering/
│
├── task-3.ipynb
├── used_cars.csv
├── cleaned_used_cars.csv
└── README.md
```

---

# 📌 Conclusion

This project demonstrates the importance of exploratory data analysis, data cleaning, and feature engineering as essential steps in the machine learning pipeline. The resulting cleaned dataset and engineered features provide a strong foundation for developing accurate used car price prediction models.
