# Laptop-Price-Analysis-Using-Python
Developed a regression model to predict laptop prices based on brand, RAM, and display specs, providing actionable insights for pricing in e-commerce and retail.
#  Laptop Price Analysis Using Python

Developed a regression model to predict laptop prices based on brand, RAM, and display specs, providing actionable insights for pricing in e-commerce and retail.

---

## Objective
Analyze a laptop dataset to identify key factors influencing prices and build a regression model to accurately predict laptop prices.

---

##  Dataset
Includes information on:
- Brand
- RAM
- Weight
- Touchscreen
- IPS Panel
- Screen Size & Resolution
- CPU, GPU
- HDD/SSD Storage
- Operating System
- Price (target variable)

---

## 🛠 Tools & Technologies
- Python (pandas, numpy)
- Jupyter Notebook
- Data Visualization: matplotlib, seaborn
- Machine Learning: scikit-learn (Linear Regression)
- Model Saving: pickle

---

##  Key Steps
- **Data Preprocessing:**
  - Converted RAM, Weight, and Screen Size to numeric types.
  - Parsed screen resolution to calculate Pixels Per Inch (PPI).
  - Encoded categorical variables (Brand, OS, CPU).
  - Removed outliers and handled missing data.

- **Exploratory Data Analysis (EDA):**
  - Analyzed relationships between features and price.
  - Generated count plots, box plots, scatter plots, and heatmaps.

- **Model Building:**
  - Built a Linear Regression model using selected features.
  - Split data into training/testing sets.
  - Achieved performance metrics:
    - R² Score: ~0.74
    - RMSE: ~354

- **Visualization:**
  - Actual vs. Predicted Prices scatter plot, highlighting model performance.

---

##  Model Saving
Trained model saved with pickle for future price predictions:
```python
import pickle
with open('Laptop_Price_Predictor.pkl', 'wb') as file:
    pickle.dump(model, file)
