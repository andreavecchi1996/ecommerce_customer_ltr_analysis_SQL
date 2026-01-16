# E-commerce customer lifetime value analysis
### Project Overview & Business Value
Fecom Inc. is an e‑commerce marketplace with many one‑time buyers. The company wants to reduce churn and stop wasting marketing budget on low‑value customers. This project utilises its CRM data to identify which countries and sellers attract customers who return (for second orders) and generate the highest lifetime revenue, allowing Fecom to determine where to allocate spending and where to invest more.


Key Questions Answered:
1. Which countries have the highest percentage of returning customers?
2. Which countries generate the highest lifetime revenue per customer?  
3. Which product categories drive lifetime revenue in top markets?

The SQL queries (data quality checks, business questions and charts) are contained in this Jupyter notebook [here](ecommerce_customer_ltv_analysis.ipynb).

# Data Structure & Initial Checks
This analysis uses four tables from Fecom Inc.'s BigQuery CRM: customer_list, orders, order_items, and products, with a total row count of roughly 300k records.

<img width="656" height="598" alt="Image" src="https://github.com/user-attachments/assets/0a826770-15af-48c9-a48c-02ab8cdf0881" />

Before analysis, the BigQuery tables were loaded into Jupyter notebooks to verify correct data ingestion and format. Quality checks and initial SQL queries for exploration are included in the notebook in the [Data Selection](ecommerce_customer_ltv_analysis.ipynb#data-selection) section.

# Executive Summary
## Overview of Findings

### Which countries have the highest percentage of returning customers?
  
Finland and Croatia currently have the highest share of customers who place at least a second order, with Finland above 5% returning customer rate.
<img width="1090" height="699" alt="Image" src="https://github.com/user-attachments/assets/5af3a818-d030-4574-bfe3-a672524cd275" />

### Which countries generate the highest lifetime revenue per customer (LTR)?
  
Based on this query, Slovakia, Luxembourg, and Finland have the highest lifetime revenue per customer. Slovakia stands out because it combines a high average LTR with a relatively large customer base (around 530 customers) and a total revenue of about 115k, compared with the much smaller bases in Luxembourg and Finland.

<img width="651" height="453" alt="Image" src="https://github.com/user-attachments/assets/fb0f88bd-150e-4ab4-a40d-2b4755f60011" />



<img width="631" height="433" alt="Image" src="https://github.com/user-attachments/assets/bfaa4b95-2bd5-4bff-8e6c-7fcf3baf2065" />
<img width="631" height="433" alt="Image" src="https://github.com/user-attachments/assets/7c28db8a-b34c-45da-8671-0d38aa8f8625" />


















---
https://www.kaggle.com/datasets/cemeraan/fecom-inc-e-com-marketplace-orders-data-crm

