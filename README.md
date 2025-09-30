# Diwali Sales Analysis Project

## Project Overview
The aim of this project is to analyze **Diwali sales** according to customer demographics such as **age, gender, and region**, in order to provide insights that can help improve sales strategies in the future.

This project focuses on understanding customer behavior during the Diwali season and identifying key target demographics for marketing and product positioning.

---

## Libraries Used
- `pandas` – for data manipulation  
- `numpy` – for numerical operations  
- `matplotlib` – for data visualization  

---

## Dataset
- File: `diwali_sales.csv` (from Kaggle)  
- Shape: **11251 rows x 15 columns**  
- Columns:  
  `User_ID, Cust_name, Product_ID, Gender, Age Group, Age, Marital_Status, State, Zone, Occupation, Product_Category, Orders, Amount, Status, Unnamed1`  

**Data Notes:**  
- Columns `Status` and `Unnamed1` contained only NaN values.  
- Marital_Status values: `0 = Non-married`, `1 = Married`.  
- Most purchased products were from the **Auto** category (based on `df.head()` and `df.tail()`).

---

## Data Cleaning
1. Converted `Marital_Status` values: `0 → Non-married`, `1 → Married`.  
2. Dropped `Status` and `Unnamed1` columns (all NaN).  
3. Renamed column `Zone` → `Region`.  
4. Checked for null values → none found. Dropped any remaining nulls.  

**Final dataset:** 11239 rows x 13 columns  

---

## Data Visualization

### 1. Average Spending by Age Group (Line Plot)
This chart highlights the **age groups with the highest average spending**, providing valuable insights into consumer behavior.  
- **Insight:** Age groups **51–55** and **36–45** spend the most.  
- Spending declines sharply for **46–50**, and is lowest for **0–17** (dependent on parents/guardians).

### 2. Gender-Based Spending Trends Across Age Demographics (Line Plot)
This chart shows how spending varies by **age group and gender**.  
- **Insight:**  
  - Females spend more in **ages 27–50**.  
  - After 50, spending rises among males.

### 3. Regional Spendings (Pie Chart)
This chart illustrates **spending patterns across regions**.  
- **Insight:** Spending is fairly uniform across regions, with **Southern region** slightly higher at **21.4%** of total spending.

### 4. Average Spending by Product Category (Horizontal Bar Chart)
This chart compares **product categories based on total spending**.  
- **Insight:**  
  - **Auto** category has the highest spending.  
  - **Office** category has the lowest spending, likely due to lower purchase frequency during vacations.

---

## Conclusions & Recommendations
- **Target Age Groups:** Focus on **51–55** and **36–45** for higher spending potential.  
- **Gender Focus:**  
  - Younger females (27–50) are key buyers.  
  - Males above 50 are important for targeted campaigns.  
- **Regional Strategy:** While spending is fairly even, the **Southern region** shows slightly higher spending.  
- **Product Categories:**  
  - **Auto** and **Tupperware** are top categories.  
  - **Office supplies** have low spending, possibly due to seasonal factors.

**Recommendation:** Sellers should target **older males (50+)** and **younger females**, with promotional focus on **Auto and Tupperware products** to maximize sales during Diwali.

---

 
