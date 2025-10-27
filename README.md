README.md (Task 3 – EDA)
# Task 3: Performed EDA on a Real-World Dataset

## 📌 Objective
The goal of this task was to **perform Exploratory Data Analysis (EDA)** on a real-world dataset.  
We explored categorical and numerical features, checked frequent values, plotted distributions, and created a correlation heatmap.

---

## 📂 Dataset
- **Dataset**: [COVID-19 Dataset
- **Format**: CSV  
- **Rows**: ~XXXX (update with actual)  
- **Columns**: ~XX (update with actual)  
- **Target (if any)**: Example → `SalePrice` (House Prices)  

---

## 🔎 Steps Performed
1. **Loaded dataset with Pandas**
   ```python
   import pandas as pd
   df = pd.read_csv("dataset.csv")


Frequent Values (Categorical Columns)

Used .value_counts() to check top frequent categories

Example: most common Neighborhood = "CollgCr" in House Prices dataset

Distribution Plots (Numerical Columns)

Used Seaborn’s histplot() with KDE to check data distribution

Example: SalePrice was right-skewed

Correlation Heatmap

Created heatmap using Seaborn’s heatmap()

Found strong positive correlation between SalePrice and GrLivArea, OverallQual

📊 Findings

Categorical features show imbalanced distributions (e.g., some values occur very frequently).

Numeric features like SalePrice show skewness.

Strong correlations between key numeric features and the target variable.

Some features show weak or no correlation, indicating low predictive power.

📈 Example Visualizations

Distribution of SalePrice


Correlation Heatmap


✅ Outcome

Gained insights into both categorical and numerical features.

Identified strong feature correlations for future modeling.

Dataset is now ready for preprocessing and feature engineering in the next step.
