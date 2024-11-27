# Business Data Management Capstone Project

## Improving Performance through Customer Segmentation and Shipping Cost Optimization: A Case Study on Walmart

### Submitted by: Kulkarni Amit Dilip  
**Roll Number:** 23f1001947  
**Program:** IITM BS Degree, Indian Institute of Technology, Madras  
**Submission Date:** November 27, 2024  

---

## Project Overview

This project focuses on analyzing Walmart's retail sales operations in the United States, addressing two key challenges:
1. **Shipping Cost Optimization** – Reducing shipping expenses by optimizing shipping modes based on order characteristics and priority.
2. **Customer Segmentation and Retention** – Enhancing customer engagement and retention through targeted marketing strategies based on customer segmentation.

### Objectives
- **Optimize Shipping Costs** to improve profit margins while maintaining timely deliveries.
- **Segment Customers** to provide tailored marketing strategies and enhance customer satisfaction.

---

## Dataset

The project uses the **Walmart Retail Sales Data** sourced from [data.world](https://data.world/ahmedmnif150/walmart-retail-dataset/).  
- **Size:** 1,037,247 rows, 23 features  
- **Key Features:**  
  - `city`: The city where the order was placed  
  - `customer_age`: Age of the customer  
  - `order_priority`: Priority level of the order (Critical, High, Medium, Low)  
  - `ship_mode`: Shipping method (Regular Air, Express Air, Delivery Truck)  
  - `unit_price`: Price per unit of the product  
  - `shipping_cost`: Cost of shipping each order  

---

## Methodology

### 1. **Data Cleaning & Preprocessing**
- Removed invalid or missing data.
- Converted object-type columns to numerical or datetime types.
- Scaled numerical features and encoded categorical variables for machine learning models.

### 2. **Exploratory Data Analysis (EDA)**
- **Correlation Analysis:** Identified significant correlations between shipping cost, unit price, and order quantity.
- **Visualization:** Used bar charts, scatter plots, and line graphs to understand patterns and relationships in the data.

### 3. **Shipping Cost Optimization**
- **Model Used:** Ridge Regression (L2 regularization)  
- **Key Insights:**  
  - Higher-priced items incur higher shipping costs due to handling and logistics.
  - Order quantity has a smaller but notable impact on shipping expenses.
- **Performance:**  
  - Mean Absolute Error (MAE): 968.80  
  - R² Score: 0.5623  

### 4. **Customer Segmentation**
- **Clustering Algorithm:** K-means clustering  
- **Features Used:** Customer age, order quantity, sales, profit, and product category.  
- **Cluster Characteristics:**  
  - **Cluster 0:** Younger customers, high order quantities, moderate sales.  
  - **Cluster 4:** Mid-age customers, high sales, and interest in Technology and Office Supplies.  
  - Other clusters exhibited distinct purchase behaviors and profit levels.

---

## Key Findings

### 1. **Shipping Cost Optimization**
- **Critical Orders:** Express Air is cost-effective for urgent deliveries.  
- **High Priority Orders:** Regular Air provides significant savings without compromising delivery speed.  
- **Medium & Low Priority Orders:** Delivery Truck is the most cost-effective option.  

### 2. **Customer Segmentation**
- Younger customers (Cluster 0) favor Office Supplies, while high-value customers (Cluster 4) prefer Technology.  
- Older customers (Clusters 1 and 3) purchase smaller quantities but consistently, indicating potential for loyalty programs.

---

## Recommendations

1. **Bulk Shipping & Negotiated Rates:** Implement bulk shipping and negotiate rates for high-value items.  
2. **Targeted Marketing:**  
   - **Cluster 0:** Introduce loyalty programs and small-business discounts.  
   - **Cluster 4:** Offer exclusive product releases and bulk purchase discounts.  
3. **Tiered Shipping Policy:**  
   - **Critical Orders:** Use Express Air for timely delivery.  
   - **High Priority Orders:** Shift to Regular Air for cost savings.  
   - **Medium & Low Priority Orders:** Use Delivery Truck for bulk items to reduce expenses.

---

## Conclusion

This project provides a strategic framework to enhance operational efficiency and customer engagement for Walmart. By optimizing shipping costs and implementing targeted marketing strategies, Walmart can improve profitability and customer satisfaction.

---

## Files in the Repository

- `Proposal.pdf`: Project proposal with background, objectives, and expected outcomes.  
- `Final_Report.pdf`: Detailed final report with analysis, findings, and recommendations.  
- `Presentation.pptx`: Project presentation summarizing the key insights and outcomes.

---

## Acknowledgments

Special thanks to [data.world](https://data.world/) for providing the dataset and the faculty of IITM BS Degree for their guidance throughout this project.
