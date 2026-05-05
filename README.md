# My-E-Commerce-ML-Project
End-to-end ML project on Pakistan’s largest ecommerce dataset including data cleaning, feature engineering, XGBoost model (95% accuracy), and interactive Plotly visualizations to predict and analyze best-selling product categories and business insights.
# Pakistan Largest Ecommerce Dataset Analysis & ML Project

This project explores and analyzes Pakistan’s largest ecommerce dataset, followed by preprocessing, feature engineering, machine learning modeling, and data visualization to predict the best-selling product categories.

---

## Project Workflow

### 1. Data Loading
- Imported large ecommerce dataset using Pandas

---

### 2. Data Cleaning
- Removed unnecessary unnamed columns
- Dropped irrelevant features (dates, IDs, etc.)
- Handled missing values using forward fill (`ffill`)
- Removed sparse rows using threshold filtering

---

### 3. Feature Engineering
- Label encoding for categorical variables:
  - status
  - sku
  - category_name_1
  - payment_method
  - BI Status
- Converted categorical data into numeric form

---

### 4. Data Scaling
- Applied StandardScaler on:
  - price
  - qty_ordered
  - grand_total

---

### 5.  Outlier Handling
- Detected outliers using Z-score method
- Replaced extreme values with median values

---

### 6.  Machine Learning Model
- Model: XGBoost Classifier
- Target: `category_name_1`
- Train-test split (80/20)
- Achieved ~95% accuracy

---

### 7.  Visualization (Plotly Express)
Performed interactive analysis using:

-  Top-selling categories (quantity & revenue)
-  Revenue distribution per category
-  Price distribution across categories
-  Order status distribution
-  Payment method trends
-  Discount impact on sales

---

## Key Insights

- Certain categories dominate both revenue and quantity sold  
- Discounts significantly influence purchase behavior  
- Payment methods vary across product categories  
- Data preprocessing greatly improved model performance  

---

##Tech Stack

- Python  
- Pandas & NumPy  
- Scikit-learn  
- XGBoost  
- Plotly Express  
- Seaborn & Matplotlib  

---

## Conclusion

This project demonstrates a full end-to-end machine learning pipeline:
from raw data cleaning → feature engineering → model training → evaluation → visualization.

---

## Future Improvements

- Hyperparameter tuning for better accuracy  
- Deployment using Streamlit or Flask  
- Real-time prediction dashboard  
- Advanced feature selection techniques  
