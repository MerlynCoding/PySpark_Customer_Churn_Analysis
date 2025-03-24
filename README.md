# PySpark_Customer_Churn_Analysis

# 📊 **Customer Churn Rate Analysis using PySpark**

## 🚀 **Project Overview**

This project demonstrates how to process and analyze customer churn data using **PySpark**, focusing on calculating **churn rates by group** (e.g., payment method). The workflow includes data preprocessing, aggregation, and visualization to provide actionable business insights for customer retention strategies.

---

## 🧰 **Tech Stack**

- **PySpark** (Spark DataFrames & SQL functions)
- **Pandas** (for local analysis and plotting)
- **Matplotlib** (for visualizations)
- **Jupyter Notebook**

---

## 📂 **Dataset**

The dataset used is the **Telco Customer Churn dataset**, containing customer-level information such as:
- Customer ID
- Churn status
- Payment Method
- Contract Type
- Monthly Charges
- Tenure, etc.

---

## 🛠️ **Key Steps Performed**

1. **Spark Session Setup**
   - Initialized PySpark environment for large dataset processing.

2. **Data Cleaning**
   - Handled NULLs in the churn column.
   - Converted "Yes"/"No" churn status to binary (1/0).

3. **Segmentation Analysis**
   - Calculated churn rate by **Payment Method**:
     \[
     \text{Churn Rate} = \left( \frac{\text{Churned Customers in Group}}{\text{Total Customers in Group}} \right) \times 100
     \]

4. **Aggregation with PySpark**
   - Used `groupBy()`, `sum()`, and `count()` to aggregate churn counts and total customers.

5. **Visualization**
   - Created bar plots using **Matplotlib** to visualize churn rates by group.

---

## 📊 **Key Insights**

- Payment methods like **Electronic Check** had a higher churn rate compared to **Credit Card Auto-pay** customers.
- Group-level churn rates provide clear signals for targeting customer retention efforts.

---

## 🔍 **Sample Output**

| Payment Method       | Churned Customers | Total Customers | Churn Rate (%) |
|----------------------|-------------------|-----------------|----------------|
| Electronic check     | 430               | 1000            | 43.0%          |
| Credit card (auto)   | 200               | 1500            | 13.3%          |
| Mailed check         | 160               | 800             | 20.0%          |

---

## 📈 **Visualization**

![Churn Rate Bar Chart](./images/churn_rate_payment_method.png)

---

## 🙌 **What I Learned**

- How to apply **grouped aggregations** with PySpark.
- Converting Spark DataFrames to Pandas for easier plotting.
- Best practices for handling missing values in Spark.
- How to calculate churn rates by different segments.

---

## 💡 **Next Steps**

- Segment churn by **Contract Type** or **Geographic Region**.
- Automate the churn rate pipeline using **Airflow**.
- Apply Spark **MLlib** for churn prediction modeling.

---

## 🧑‍💻 **Author**

**James** | Junior Data Analyst  
_This project was part of my hands-on practice with PySpark and data visualization._

---
