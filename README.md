# 📊 Sales Insights Dashboard

This repository showcasesA comprehensive Sales Insights of a company Dashboard built using Power BI, providing key metrics and visualizations to analyze sales performance effectively. This project showcases data analytics and visualization skills, enabling informed decision-making for business growth.
---
### Data Analysis Using SQL
SQL database dump is in db_dump.sql file above. Download `db_dump_Data.sql` file to your local computer and import in mysql.
1. Show all customer records

    `SELECT * FROM customers;`

1. Show total number of customers

    `SELECT count(*) FROM customers;`

1. Show transactions for Chennai market (market code for chennai is Mark001

    `SELECT * FROM transactions where market_code='Mark001';`

1. Show distrinct product codes that were sold in chennai

    `SELECT distinct product_code FROM transactions where market_code='Mark001';`

1. Show transactions where currency is US dollars

    `SELECT * from transactions where currency="USD"`

1. Show transactions in 2020 join by date table

    `SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;`

1. Show total revenue in year 2020,

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";`
	
1. Show total revenue in year 2020, January Month,

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and and date.month_name="January" and (transactions.currency="INR\r" or transactions.currency="USD\r");`

1. Show total revenue in year 2020 in Chennai

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020
and transactions.market_code="Mark001";

## 🌟 Key Highlights On DashBoard:

### **1. Revenue Analysis**
- **Total Revenue **: - **984.81M**  
- **Revenue in year 2017 **: - **92.88M**
- **Revenue by Month**:
  - **Revenue in Jan 2019** : -  **31.53M**

### **2. Top Products Sales **
- ** This visualization highlights the top 5 performing products based on sales revenue or quantity sold. It provides a quick overview of the most successful products, helping businesses identify key contributors to their sales performance.**:
- ** It Helps:
Recognize trends in customer preferences.
Focus on high-demand products for inventory planning.
Create targeted marketing campaigns for top products.
  **

### **3. Top Buying Customers**
#### Insights:  
- Recognize the **highest-spending customers** contributing to overall sales.  
- Focus on VIP customers for loyalty programs and personalized campaigns.  
- Understand buying patterns to enhance customer retention strategies.  

#### Interactive Features:  
- **Filters**: Adjust by time period, region, or product category to analyze specific trends.  
- **Tooltips**: Hover over the bars to see detailed metrics.  

### **4. Geographic and Demographic Insights**
#### Insights:  
- Pinpoint **top-performing regions** to focus marketing and distribution efforts.  
- Understand customer demographics to tailor product offerings and campaigns.  
- Detect opportunities for expansion in underperforming regions.  

#### Interactive Features:  
- **Filters**:  
  - Adjust by product categories, time periods, or regions to explore trends dynamically.  
- **Tooltips**: View detailed metrics for regions or demographic groups by hovering over visual elements. 

---

## 📈 Key Performance Indicators (KPIs)
- **Total Revenue**: **984.81M**
- **Total Sales Quantity**: **2M**
- **Total time Period**: **4years**

---

## 🛠 Tools and Technologies
- **Power BI**: Interactive data visualization and dashboard creation.
- **Data Sources**: Sales Data of a Company.
- **Key Features**: Drill-through functionality, slicers, and KPI metrics.

---

## 🚀 Getting Started

### **Prerequisites**
1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Download the `.pbix` file from this repository.

### **Steps to Explore**
1. Open the `.pbix` file in Power BI Desktop.
2. Interact with dynamic filters, charts, and KPIs to explore the data.

---

## 📷 Dashboard Preview
![image](https://github.com/user-attachments/assets/3a07ae70-7c31-42bc-a002-84ec2eca5f5e)

## Report in Year 2020:
![image](https://github.com/user-attachments/assets/519e270e-042a-4a48-8a9a-8f1cbeb674b9)

---


### 🌟 If you find this project useful, don't forget to give it a ⭐ on GitHub!
