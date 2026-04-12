# Experiment 14 - Data Normalization and Data Type Conversion

## Overview
This experiment explores the essential preprocessing steps required to prepare raw datasets for machine learning and statistical analysis. We focus on two primary pillars: **Data Normalization**, which standardizes numerical ranges to prevent feature bias, and **Data Type Conversion**, which transforms categorical labels into machine-readable formats.

## Objectives
* Apply mathematical scaling techniques to external datasets.
* Execute categorical encoding using the `Scikit-Learn` framework.
* Understand the impact of outliers on various normalization strategies.

## Tools & Environment
* **Environment:** Google Colab / Jupyter Notebook
* **Key Library:** `Scikit-Learn` (specifically the `preprocessing` module)

---

## Technical Theory

### 1. Data Normalization Strategies
Normalization ensures that features with large magnitudes do not dominate those with smaller scales during model training.

* **Min-Max Scaling:** Linearly transforms data into a fixed range (usually 0 to 1). While simple, it is highly sensitive to outliers.
    $$x' = \frac{x - \min(x)}{\max(x) - \min(x)}$$
* **Z-Score Standardization:** Re-scales data based on the mean ($\mu$) and standard deviation ($\sigma$). This is ideal for datasets with outliers as it does not bound the data to a specific range.
    $$z = \frac{x - \mu}{\sigma}$$
* **Decimal Scaling:** Shifts the decimal point based on the maximum absolute value in the feature set.
    $$x' = \frac{x}{10^j}$$

### 2. Data Type Conversion & Encoding
Since most mathematical models cannot interpret text strings, we use encoding to translate categorical variables into numerical values.

* **Label Encoding:** Assigns a unique integer (0, 1, etc.) to each category. Best used for ordinal data or binary classifications.
* **One-Hot Encoding (OHE):** Creates separate "dummy" columns for every unique category. A value of `True` (or 1) indicates the presence of that category.
* **Dummy Encoding:** A variation of OHE where one category is dropped (`drop_first=True`) to avoid the "dummy variable trap" (multi-collinearity).

---

## Implementation via Scikit-Learn
The `sklearn.preprocessing` module provides the standard tools for these transformations:

| Method | Implementation Snippet |
| :--- | :--- |
| **Label Encoding** | `from sklearn.preprocessing import LabelEncoder; le = LabelEncoder()` |
| **One-Hot Encoding** | `pd.get_dummies(df, columns=['Feature'])` |
| **Dummy Encoding** | `pd.get_dummies(df, drop_first=True)` |

---

## Practical Applications
* **IoT & Sensors:** Converting raw string data from hardware sensors into `float` types for real-time logic execution.
* **Equity Markets:** Normalizing share prices so that expensive stocks and penny stocks can be compared on the same scale for volatility analysis.
* **Recommendation Engines:** Standardizing user ratings to account for "strict" vs. "lenient" reviewers.

## Key Takeaways
* **Efficiency:** Normalized data allows optimization algorithms like Gradient Descent to converge significantly faster.
* **Integrity:** Proper encoding prevents the model from assuming a false numerical hierarchy in categorical data (e.g., assuming "Red" is greater than "Blue").
* **Consistency:** Data type conversion ensures that mathematical operations can be performed without format errors.

## Conclusion
This experiment successfully demonstrated how to clean and restructure datasets using normalization and encoding. By applying these techniques via `Scikit-Learn`, we ensure that our data is both mathematically consistent and ready for high-performance modeling.
