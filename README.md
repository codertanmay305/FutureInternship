# FutureInternship

##Task 1

# 📊 Superstore Sales Forecasting Project

## 📝 Overview
This project was completed as part of the **Future Interns Machine Learning Internship**. The objective of the project was to build a predictive model to forecast retail sales for a **Superstore** using historical sales data from **2014–2017**.

The goal of this analysis is to generate actionable insights that help businesses make better decisions related to:

- 📦 Inventory management  
- 💰 Cash flow optimization  
- 👥 Staffing requirements  

By forecasting future sales, businesses can better prepare for demand fluctuations and optimize operations.

---

## 🎯 Project Objectives
The main objective of this project was to forecast **monthly sales for the next six months (January – June 2026)**. This helps answer several important business questions:

### 📦 Inventory
- When should new stock be ordered based on supplier lead times?

### 💰 Cash Flow
- When will revenue be low?
- When will the business generate higher revenue that can be saved?

### 👥 Staffing
- When will the warehouse require additional staff to manage order surges?

---

## 🛠️ Data & Methodology

### 1️⃣ Data Source
The project uses the **Superstore Sales Dataset**, which contains transaction data between **2014 and 2017**.

The dataset includes information such as:
- Order date
- Product category
- Sales amount
- Customer details
- Shipping information

This data was cleaned, processed, and transformed before being used for machine learning modeling.

---

### 2️⃣ Predictive Modeling
Two machine learning models were implemented and compared to determine the best forecasting approach.

#### Linear Regression (LR)
- Performs well in detecting **large sales spikes**
- Example: Captured the significant surge in **November 2017 (~$118k)**

#### Random Forest (RF)
- Produces more **stable and conservative predictions**
- Avoids large overestimations during stable sales periods

---

### 3️⃣ Final Model Selection
To produce more balanced predictions, the final forecast combines insights from both models.

**Estimated Model Accuracy:**  
Approximately **80%**

---

## 📈 Key Findings & Forecast (2026)

Based on the trained models, the predicted sales for the first half of **2026** are:

**Total Predicted Sales (Jan – Jun 2026):**  
💰 Approximately **$540,000**

### 📉 Lowest Sales Month
**February 2026**  
Estimated sales: **~$78,945**

### 📈 Highest Sales Month
**June 2026**  
Estimated sales: **~$102,346**

These forecasts provide useful insights for operational and financial planning.

---

## 💡 Business Impact & Action Plan

### 📦 Inventory Management
**Technology Category (28% of total sales)**  
Products such as **phones and copiers** require **4–6 weeks lead time**.

Recommendation:
- Place orders **by mid-April** to prepare for the **June demand peak**.

**Furniture Category**
- Requires **6–8 weeks lead time**
- Orders should be finalized **by March**.

---

### 💰 Finance & Cash Flow Planning
Sales typically decrease after the holiday season, especially during **February and March**.

Recommendation:
- Build financial reserves during **high-revenue months like June** to support slower periods.

---

### 👥 HR & Operations

**Staffing Strategy**
- Hire **2–3 temporary warehouse workers by May 1st**.

**Training Plan**
- Complete **weekend staff training by May 15th** to prepare for the June order surge.

---

## ▶️ How to Run the Project

```bash
1️⃣ Clone the repository
git clone https://github.com/codertanmay305/superstore-sales-forecasting.git

2️⃣ Navigate to the project folder

cd superstore-sales-forecasting

3️⃣ Install the required libraries

pip install pandas scikit-learn matplotlib seaborn jupyter

4️⃣ Open the Jupyter Notebook

jupyter notebook
