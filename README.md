# E-commerce_Data_Pipeline-Pricing_Analysis

https://app.powerbi.com/Redirect?action=OpenReport&appId=ccac07f0-05a1-4cf5-b4e6-a4f104208353&reportObjectId=cbac72c5-2b29-4bb4-ba2a-8456d264bc6f&ctid=fd0853e9-4432-4693-8bd9-5cac61a80641&reportPage=61042cf049c302d54398&pbi_source=appShareLink&portalSessionId=d51a7ba8-940d-47af-8555-28b4fc4cd038

## 📌 Project Background

Retail datasets are often messy, inconsistent, and incomplete, making them difficult to analyze directly.  
This project focuses on building an **end-to-end data pipeline** to ingest, clean, transform, and analyze e-commerce data for men's shirts.

The dataset (~1450 records) contains product-level information including **brand, product title, original price, and sale price**.

The objective is to simulate a real-world scenario where raw retail data is processed into a structured format to enable **pricing, discount, and brand-level analysis**.

---

## 📈 Executive Summary

This project demonstrates how raw retail data can be transformed into actionable insights through structured data engineering and visualization.

<img width="1920" height="899" alt="Screenshot (1895)" src="https://github.com/user-attachments/assets/d2d953cb-fb38-48db-9c50-e38491cd8f3e" />

The analysis reveals that **top-selling brands are not necessarily the ones offering the highest discounts**, indicating that factors such as brand value and product positioning play a critical role in sales performance.

Additionally, a small number of brands dominate product variety, suggesting **market concentration**, while aggressive discounting is primarily observed among less dominant brands.

Overall, the project highlights the importance of **clean data pipelines and structured transformations** in enabling meaningful retail analysis.

---

## 🔍 Key Insights

<img width="1920" height="899" alt="Screenshot (1895)" src="https://github.com/user-attachments/assets/d2d953cb-fb38-48db-9c50-e38491cd8f3e" />

### 1. Top-Selling Brands Are Not Discount Leaders
- Brands like **Armani Exchange (140K)** and **US Polo Association (135K)** lead in sales  
- However, they are NOT among the highest discount providers  

👉 Indicates **brand strength > discounting strategy**

---

### 2. High Discount ≠ High Sales
- Brands offering highest discounts (e.g., iVOC ~89%) do not appear in top sales  

👉 Suggests **discounting alone is not sufficient to drive revenue**

---

### 3. Market is Highly Concentrated
- **The Indian Garage Co contributes ~42% of total product variety (184 products)**  
- Followed by US Polo (24%) and Netplay (20%)

👉 Indicates **few brands dominate inventory presence**

---

### 4. Mid-Tier Brands Compete on Pricing
- Brands outside top sellers offer significantly higher discounts (80%+)

👉 Likely strategy:
- Compete on **price rather than brand positioning**

---

### 5. Sales Leadership is Brand-Driven
- Top 5 brands contribute a major share of total sales

👉 Suggests **customer preference is skewed toward established brands**

---

### 6. Data Quality Challenges Required Intervention
- Missing values in price columns were handled using **imputation (0.7 × sale price)**  
- Special characters (₹ symbol issues) were cleaned at the database level  

👉 Highlights importance of **data preparation before analysis**

---

## 💡 Recommendations

### 1. Optimize Discount Strategy
- Avoid excessive discounting without clear impact on sales  
- Focus on **value-based pricing instead of deep discounts**

---

### 2. Strengthen Brand Positioning
- Sales leaders succeed with lower discounts → invest in branding  

---

### 3. Diversify Product Portfolio
- Reduce dependency on a few dominant brands  
- Expand offerings across underrepresented brands  

---

### 4. Improve Data Collection Standards
- Ensure consistent price formatting  
- Minimize missing values at source  

---

## 🛠️ Tech Stack Used

- **Data Source**: CSV File  
- **Database**: Azure SQL Database  
- **Query Tool**: SQL Server Management Studio (SSMS)  
- **Data Cleaning & Transformation**: SQL + Power Query  
- **Visualization**: Power BI Desktop  
- **Deployment**: Power BI Service  

---

## ⚙️ Data Pipeline Overview

1. Created Azure SQL Database and connected via SSMS  
<img width="1920" height="915" alt="Screenshot (1884)" src="https://github.com/user-attachments/assets/ce55541c-2ce3-438d-95c2-2cacb5aea1b2" />

2. Imported raw CSV data into database  
3. Cleaned data using SQL:
<img width="1920" height="907" alt="Screenshot (1889)" src="https://github.com/user-attachments/assets/4b7fe3b5-c885-4ec5-98ee-4705503a1cca" />

   - Removed special characters from price columns  
4. Loaded data into Power BI  
<img width="1920" height="965" alt="Screenshot (1890)" src="https://github.com/user-attachments/assets/627ec923-2e77-4d0d-a8b3-64b13097cfdb" />

5. Performed transformations:
   - Handled missing values via imputation  
   - Converted data types  
6. Built calculated columns:
   - Discount %  
   - (Simulated) Profit %  
   - Cost Price  
7. Developed interactive dashboard  
8. Published report to Power BI Service  

---
https://app.powerbi.com/Redirect?action=OpenReport&appId=ccac07f0-05a1-4cf5-b4e6-a4f104208353&reportObjectId=cbac72c5-2b29-4bb4-ba2a-8456d264bc6f&ctid=fd0853e9-4432-4693-8bd9-5cac61a80641&reportPage=61042cf049c302d54398&pbi_source=appShareLink&portalSessionId=d51a7ba8-940d-47af-8555-28b4fc4cd038
## 📊 Key Takeaway

This project demonstrates that **cleaning and structuring data is as important as analysis itself**, and that meaningful insights depend on how well raw data is prepared and interpreted.

---
