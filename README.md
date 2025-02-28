# Sales Analysis Insights for Ferns and Petals (FNP) (Excel project)

## Overview
This document provides insights derived from the sales analysis dashboard of Ferns and Petals (FNP). The data highlights key trends in revenue, order distribution, and product performance. The analysis is based on the provided dashboard, focusing on total revenue, order trends, customer spending, and sales distribution.


![Screenshot 2025-02-28 021248](https://github.com/user-attachments/assets/06c3670e-cffd-48ef-90c7-c31339be0a28)


---

## Key Insights

### 1. **Overall Performance**
- **Total Revenue:** $3,520,984
- **Total Orders:** 1,000
- **Average Days of Delivery:** 5.53 days
- **Average Customer Spend:** $3,521

### 2. **Revenue Trends**
- **Revenue by Month:**
  - There are noticeable peaks in revenue during specific months, which coincide with major occasions like Diwali and Holi.
  - The highest revenue-generating months appear to be March (Holi) and October-November (Diwali).
  
- **Revenue by Hour:**
  - Peak sales occur between **10 AM and 9 PM**, indicating that most customers place orders during working hours and early evening.

### 3. **Top Products and Categories**
- **Best-selling Product Categories:**
  - **Colors, Soft Toys, Sweets, and Cakes** generate the highest revenue, indicating strong demand for gifting-related products.
  - **Plants and Mugs** have lower sales, suggesting they may require promotional boosts.

- **Top 5 Products by Revenue:**
  - **Dessert Box:** $97,685
  - **Harum Pack:** $91,558
  - **Delores Gift:** $106,634
  - **Quia Gift:** $144,476
  - **Unknown Product:** $113,905 (requires further investigation for better product naming clarity)

### 4. **Geographical Insights**
- **Top 10 Cities by Orders:**
  - The highest number of orders come from metro cities, including Delhi, Mumbai, Bangalore, Hyderabad, and Chennai.
  - The company should focus on strengthening operations in these cities to further boost sales.

### 5. **Occasion-Based Revenue**
- **Total Revenue by Occasion:**
  - **Diwali:** $574,926 (High Revenue)
  - **Holi:** $631,585 (Highest Revenue)
  - **Anniversary:** $674,843 (Top Revenue)
  - **Birthday:** $498,194
  - **Raksha Bandhan:** $313,783
  - **Valentine’s Day:** $313,930
  - **All Occasions:** $586,176
  
- **Observations:**
  - Holi and Diwali contribute significantly to total sales, demonstrating the strong cultural impact of these festivals on online gifting.
  - Raksha Bandhan and Valentine’s Day have lower sales, suggesting an opportunity for better marketing campaigns.

---

## Star Schema Structure
The sales analysis dashboard follows a **star schema** data model, which ensures optimized querying and reporting. The key tables and their relationships are as follows:

### 1. **Fact Table: orders**
   - Contains transaction-level details such as **Order_ID, Customer_ID, Product_ID, Quantity, Order_Date, Delivery_Time, Price, Revenue**, and other relevant attributes.

### 2. **Dimension Tables:**
   - **customers:** Stores customer-specific details (**Customer_ID, Name, City, Gender, Contact Details, Total Revenue**).
   - **products:** Contains product-related information (**Product_ID, Product_Name, Category, Price, Occasion, Description**).
   - **date:** Includes date-based attributes for time-series analysis (**Order_Date, Delivery_Date, Month_Name, Days_of_delivery, Order_Day**).

### 3. **Relationships:**
   - **Customers** (1) → (**Orders**) (*): Each customer can have multiple orders.
   - **Products** (1) → (**Orders**) (*): Each product can appear in multiple orders.
   - **Date** (1) → (**Orders**) (*): Each order is linked to a specific date for time-based analysis.

This schema design enables efficient data retrieval for business intelligence reporting, ensuring seamless analysis of revenue trends, customer behavior, and product performance.

![Screenshot 2025-02-18 023131](https://github.com/user-attachments/assets/37690e1b-1ac3-41e6-9f62-934b6a219bf8)

---

## Recommendations

please check finial report


