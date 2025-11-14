# Supply-and-Sale-Management-with-Business-Intelligence
A complete Business Intelligence case study for a retail chain of 44 stores, featuring star schema design, descriptive, predictive, and prescriptive analytics. Includes item and store analysis, demand forecasting, customer segmentation, new store feasibility, and recommendations to optimize sales and operations.

---

## Project Overview
This project analyzes a retail chain with 44 stores distributed across the country, each equipped with a retail management system that handles procurement, inventory, and sales. The BI workflow includes item-level, store-level, supplier-level, and customer-level analytics to support strategic decision-making.

The project performs:
- **Descriptive Analytics** – Summaries, historical trends, seasonal patterns, store performance.
- **Predictive Analytics** – Forecasting item demand, predicting store revenue, and modeling customer behavior.
- **Prescriptive Analytics** – Recommendations for inventory optimization, store expansion, marketing, and profit improvement.

---

##  Data Model & Star Schema
The retail BI model uses one fact table and several dimension tables:

### **Fact Table**
- `FactSales`: transaction-level details including item, customer, store, price, quantity, time, payment type, and bank.

### **Dimensions**
- `DimItem` – item metadata and supplier info  
- `DimStore` – store location and operational attributes  
- `DimCustomer` – demographic & socioeconomic profiles  
- `DimTime` – full time hierarchy (hour → year)

The star schema supports OLAP analysis for items, stores, suppliers, and customers.

---

##  Machine Learning Models Used
The notebook includes multiple ML techniques applied based on the analytical requirements:

### **1. Regression Models**
Used for predicting:
- Future store revenue  
- Item-wise future sales  

Models implemented:
- **Linear Regression**  
- **Multiple Linear Regression**    

### **2. Time Series Forecasting Models**
Used for demand forecasting and monthly sales prediction:
- **ARIMA / SARIMA**  
- **Moving Average / Exponential Smoothing**

### **3. Classification Models**
Used for customer segmentation, purchase prediction, and classification tasks:
- **K-Means Clustering** (unsupervised)  
- **Logistic Regression**  
- **Decision Tree Classifier**

### **4. Recommendation Logic**
(Not ML-heavy but included in prescriptive analytics)
- Rule-based recommendation engine  
- Customer cluster–based targeted advertisement strategy

---

##  Descriptive Analysis
Covers:
- Total and monthly sales trends  
- Revenue distribution across stores  
- Item-level performance  
- Supplier contribution and delivery behavior  
- Customer demographics and frequency of purchase

These insights highlight business strengths, weaknesses, and historical behavior patterns.

---

##  Predictive Analysis
Based on the ML models above, forecasts include:
- Expected demand for selected items  
- Future revenue of the assigned store  
- Prediction of whether a customer may purchase certain item categories

Predictive workflow follows the protocol described in the case study:  
Define → Explore → Model → Deploy → Validate.

---

##  Prescriptive Analysis
The project provides actionable recommendations such as:
- Reorder quantity strategies & safety stock suggestions  
- Identifying stores needing operational improvement  
- Advertisement targeting based on clusters  
- Pricing and promotional recommendations  
- Feasibility evaluation for a **New Store Location**

---

##  Customer Classification
Customers are classified based on:
- Purchase behavior  
- Income  
- Age, profession, qualification  
- Frequency and recency  

Methods used:
- K-Means Clustering  
- RFM Scoring  
- Demographic segmentation

---

##  Advertisement Recommendation
Using customer cluster profiles:
- High-income → premium imported products  
- Young customers → electronics & fast-moving items  
- Families → grocery bundles  
- Budget-conscious → deals and discounts  
- Students → mobile banking cashback offers

---

##  New Store Feasibility
Evaluated using:
- Area population  
- Store density  
- Purchasing power  
- Sales performance of nearby stores  
- Logistic accessibility  

---

## Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib/Seaborn  
- Scikit-learn
- ML models
- Statsmodels (ARIMA forecasting)  
- Google Colab
- Business Intelligence Concepts (Descriptive, Predictive, Prescriptive)

---

##  How to Run
1. Clone the repository  
2. Open the notebook in Google Colab 
3. Install required Python libraries  
4. Run all cells to generate outputs  

---
Author

Mahmud Un Nabi
Business Intelligence & Data Analytics Student- BUET 2025
