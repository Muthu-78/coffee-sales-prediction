#  Coffee Shop Sales Prediction | Linear Regression

**Predicting daily revenue using Python and Scikit-learn**  
![Python](https://img.shields.io/badge/Python-3.8%2B-blue) ![Pandas](https://img.shields.io/badge/Pandas-1.2+-brightgreen) ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-0.24+-orange)

---

## 📌 Project Overview
Linear regression model predicting daily coffee shop revenue using:
- **365 days** of historical sales data
- **26 features** (sales, weather, promotions, etc.)

**Key Techniques**:
- **Data Cleaning**: Handled missing values, outlier detection
- **Feature Engineering**:
  - Time-based features (Day_of_Year, Week_of_Year)
  - Categorical encoding (LabelEncoder)
  - Correlation-based feature selection (`SelectKBest`)
- **Modeling**: Linear Regression with `StandardScaler`
- **Evaluation**: R² (0.82), MSE (411.11), residual analysis

---

##  Dataset
**File**: `coffee_shop_sales_dataset.xlsx`  
**Notable Features**:
- Sales metrics (Coffee, Pastry, Sandwich)
- Operational costs (Staff, Ingredients)
- External factors (Temperature, Rainfall, Holidays)

**Sample EDA**:
```python
df.describe()  # Statistical summary
sns.heatmap(df.corr())  # Feature correlations
