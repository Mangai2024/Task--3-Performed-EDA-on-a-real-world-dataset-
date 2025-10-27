README.md (Task 3 – COVID-19 Dataset EDA)
# Task 3: Performed EDA on COVID-19 Dataset

## 📌 Objective
The goal of this task was to **perform Exploratory Data Analysis (EDA)** on a real-world COVID-19 dataset.  
We explored categorical and numerical features, checked frequent values, plotted distributions, and created a correlation heatmap.

---

## 📂 Dataset Link - https://github.com/Mangai2024/Task--3-Performed-EDA-on-a-real-world-dataset-/blob/main/covid_19.csv
- **Dataset**: COVID-19 Statistics  
- **Rows**: 187  
- **Columns**: 15  
- **Important Columns**:  
  - Country/Region  
  - WHO Region  
  - Confirmed, Deaths, Recovered, Active  
  - New cases, New deaths, New recovered  
  - Ratios like Deaths / 100 Cases, Recovered / 100 Cases  

---

## 🔎 Steps Performed
1. **Loaded dataset with Pandas**
   ```python
   import pandas as pd
   df = pd.read_csv("covid_19.csv")


Frequent Values (Categorical Columns)

Checked most frequent categories using .value_counts()

Example:

WHO Region → Europe (56), Africa (48), Americas (35), Eastern Mediterranean (22), Western Pacific (16)

Distribution Plots (Numerical Columns)

Plotted histograms for:

Confirmed cases

Deaths

Recovered

Active

New cases

All distributions showed right skewness (most countries had low counts, few had very high).

Correlation Heatmap

Used Seaborn heatmap() on numeric columns

Strong correlations found:

Confirmed ↔ Deaths (positive correlation)

Confirmed ↔ Recovered (very strong correlation)

New cases ↔ New deaths (moderate correlation)

📊 Findings

Categorical: Europe and Africa dominate the WHO region counts.

Numeric: Confirmed, Deaths, and Recovered all show skewed distributions.

Correlation: Confirmed cases strongly drive both deaths and recoveries.

📈 Example Visualizations

Distribution of Confirmed Cases


Correlation Heatmap


✅ Outcome

Performed EDA on a real-world COVID-19 dataset.

Identified categorical distributions, numeric feature patterns, and feature correlations.

Dataset is now ready for further preprocessing and modeling tasks.
