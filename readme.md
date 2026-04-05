# 🛍️ Customer Shopping Behavior Analysis

## 📌 Project Overview
This project analyzes customer shopping behavior using transactional data from **3,900 purchases** across multiple product categories.

The goal is to uncover insights into:
- Customer spending patterns  
- Product preferences  
- Subscription behavior  
- Customer segmentation  

These insights help businesses make **data-driven decisions**.

---

## 📊 Dataset Summary
- **Total Records:** 3,900  
- **Total Features:** 18  

### Key Features:
- **Demographics:** Age, Gender, Location, Subscription Status  
- **Purchase Details:** Item Purchased, Category, Amount, Season, Size, Color  
- **Behavioral Data:** Discounts, Promo Usage, Frequency, Ratings, Shipping Type  

### Data Issues:
- 37 missing values in **Review Rating** column (handled using median imputation)

---

## 🧹 Data Preparation (Python)

- Loaded dataset using `pandas`
- Performed initial exploration using:
  - `df.info()`
  - `df.describe()`
- Handled missing values using **category-wise median**
- Renamed columns to **snake_case**
- Feature Engineering:
  - `age_group`
  - `purchase_frequency_days`
- Removed redundant column: `promo_code_used`
- Loaded cleaned data into **PostgreSQL**

---

## 🗄️ SQL Analysis

### Key Business Questions Solved:

- Revenue comparison by gender  
- High-spending customers using discounts  
- Top 5 products by rating  
- Shipping type comparison  
- Subscribers vs non-subscribers  
- Discount-dependent products  
- Customer segmentation  
- Top 3 products per category  
- Repeat buyers & subscription behavior  
- Revenue by age group  

---

## 👥 Customer Segmentation

Customers were divided into:
- **New Customers**
- **Returning Customers**
- **Loyal Customers**

> Majority of customers fall into the **Loyal segment (~80%)**

---

## 📊 Power BI Dashboard

An interactive dashboard was built to visualize insights.

### Dashboard Features:
- KPI Cards:
  - Total Customers  
  - Average Purchase Amount  
  - Average Review Rating  

- Filters:
  - Gender  
  - Category  
  - Subscription Status  
  - Shipping Type  

- Visualizations:
  - Revenue by Category  
  - Sales by Category  
  - Revenue by Age Group  
  - Sales by Age Group  

---

## 💡 Key Insights

- Male customers generated **~2x revenue** compared to female customers  
- **839 customers** spent above average even with discounts  
- **Young Adults** contribute the highest revenue  
- Express shipping users spend slightly more than standard  
- Subscription does not significantly affect average spending  

---

## 🚀 Business Recommendations

- **Increase Subscriptions**
  - Offer exclusive benefits and incentives  

- **Loyalty Programs**
  - Reward repeat buyers  

- **Optimize Discounts**
  - Maintain balance between sales and profit margins  

- **Targeted Marketing**
  - Focus on high-revenue segments  

- **Product Strategy**
  - Promote top-rated and high-selling products  

---

## 🛠️ Tech Stack

- **Python** (Pandas, Data Cleaning, EDA)  
- **PostgreSQL** (SQL Analysis)  
- **Power BI** (Dashboard & Visualization)  

---

## 📂 Project Structure
