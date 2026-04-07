# 🛒 Customer Shopping Behavior Analysis

## 📌 Project Overview
This project analyzes customer shopping behavior using transactional data from **3,900 purchases** across multiple product categories.  

The objective is to extract actionable insights on:
- Customer spending patterns  
- Product preferences  
- Subscription behavior  
- Business performance  

These insights help support **data-driven decision-making** for business growth.

---

## 📊 Dataset Summary
- **Total Rows:** 3,900  
- **Total Columns:** 18  

### Key Features:
- **Customer Info:** Age, Gender, Location, Subscription Status  
- **Purchase Details:** Item Purchased, Category, Amount, Season, Size, Color  
- **Behavioral Data:**  
  - Discount Applied  
  - Promo Code Used  
  - Previous Purchases  
  - Purchase Frequency  
  - Review Rating  
  - Shipping Type  

⚠️ Missing Data:
- 37 missing values in the **Review Rating** column (handled during preprocessing)

---

## 🐍 Exploratory Data Analysis (Python)

### Steps Performed:
- Data loading using **pandas**
- Data inspection using:
  - `df.info()`
  - `df.describe()`
- Missing value handling:
  - Imputed using **median rating per category**
- Column renaming:
  - Converted to **snake_case**
- Feature engineering:
  - Created `age_group`
  - Created `purchase_frequency_days`
- Removed redundant columns:
  - Dropped `promo_code_used`
- Integrated with **PostgreSQL** for further analysis

---

## 🗄️ SQL Analysis (PostgreSQL)

Key business questions answered:

1. Revenue comparison by gender  
2. High-spending customers using discounts  
3. Top 5 highest-rated products  
4. Shipping type vs purchase amount  
5. Subscribers vs non-subscribers analysis  
6. Discount-dependent products  
7. Customer segmentation:
   - New  
   - Returning  
   - Loyal  
8. Top 3 products per category  
9. Repeat buyers vs subscription behavior  
10. Revenue by age group  

---

## 📈 Power BI Dashboard

### Dashboard Preview
![Power BI Dashboard](https://github.com/rohit2k5/Customer-Behavior-Analysis/blob/main/Screenshot%202026-04-07%20183625.png)

---

## 💡 Business Recommendations

- ✅ Promote subscription benefits to increase retention  
- 🎯 Implement loyalty programs for repeat customers  
- ⚖️ Optimize discount strategies to protect margins  
- ⭐ Highlight top-rated & best-selling products  
- 📢 Target high-value customer segments with focused marketing  

---

## 🛠️ Tech Stack

- **Python** (Pandas, Data Cleaning, EDA)  
- **SQL (PostgreSQL)**  
- **Power BI** (Dashboard & Visualization)  

---

## 📂 Project Structure
├── data/
├── notebooks/
├── sql/
├── dashboard.png
├── README.md


---

## 🚀 How to Run

1. Load dataset into Python  
2. Perform preprocessing & cleaning  
3. Push cleaned data into PostgreSQL  
4. Run SQL queries for analysis  
5. Visualize results in Power BI  

---

## 📎 Key Learnings
- Data cleaning & preprocessing techniques  
- Feature engineering for better insights  
- Writing optimized SQL queries  
- Building business-focused dashboards  
