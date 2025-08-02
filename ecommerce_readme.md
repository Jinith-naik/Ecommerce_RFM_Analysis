# 🛒 Ecommerce Customer Segmentation using RFM Analysis

Welcome to a complete end-to-end customer segmentation project built using **Python**, **Jupyter Notebook**, and **Power BI**. This project uses **RFM Analysis (Recency, Frequency, Monetary)** to divide customers into actionable segments and help e-commerce businesses boost retention, optimize marketing, and drive growth.

---

## 👨‍💼 Author

**Jinith Naik**  
📧 jinithnaikcareer@gmail.com | 📞 +91-7990554873  
🔗 [LinkedIn](https://www.linkedin.com/in/jinithnaik)

---

## 🎯 Project Goal

**Why this project?**  
E-commerce platforms collect tons of transaction data but struggle to:
- Identify high-value customers
- Predict churn
- Design personalized retention strategies

Using RFM (Recency, Frequency, Monetary) scoring, we **segment customers** into groups and provide **custom business strategies** for each group.

---

## 📁 Repository Structure

```
.
├── Ecommerce_Data_Analysis.ipynb    # Full Python notebook with RFM analysis and plots
├── Analytics_Project2_Ecommerce.xlsx # Raw data file (original source)
├── data.csv                         # Cleaned dataset after preprocessing
├── Ecommerce_RFM_Report.pbix        # Power BI dashboard (interactive segmentation)
├── Customer Segmentation.pptx       # Executive presentation summary
├── README.md                        # This file
```

---

## 📦 Dataset Overview

| Feature      | Description                                  |
|--------------|----------------------------------------------|
| `InvoiceNo`  | Transaction ID                               |
| `StockCode`  | Product ID                                   |
| `Description`| Product description                          |
| `Quantity`   | Units purchased                              |
| `InvoiceDate`| Timestamp of purchase                        |
| `UnitPrice`  | Price per unit in GBP                        |
| `CustomerID` | Unique customer identifier                   |
| `Country`    | Country of the customer                      |

- **Source**: Kaggle E-Commerce Dataset  
- **Timeframe**: Dec 1, 2010 – Dec 9, 2011  
- **Size**: 541,909 rows × 8 columns  

---

## 🧹 Data Cleaning Summary

| Step                 | Description |
|----------------------|-------------|
| 🔍 Missing Values     | Removed 24.93% rows with missing `CustomerID` |
| 🔁 Duplicates         | Removed 5,525 duplicate rows |
| ❌ Cancelled Orders   | Removed 8,872 rows with `InvoiceNo` starting with 'C' (indicates returns) |
| 🧪 Non-Product Codes  | Removed non-product `StockCode` rows (e.g., samples, adjustments) |
| 🔢 Type Conversion    | Converted `InvoiceDate` to datetime, ensured numeric columns are floats |

✅ Cleaned data is stored in `data.csv`.

---

## 🔍 Exploratory Insights (EDA)

### 📊 Pareto Analysis (80/20 Rule)
- **26% of customers** generated **80% of revenue**
- **21% of products** contributed to **80% of sales**

💡 Business Insight: A small group of loyal customers are the major revenue drivers. Prioritize retention and loyalty rewards here.

---

## 📈 RFM Analysis Explained

### What is RFM?

| RFM Metric | Meaning                            | Importance                         |
|------------|-------------------------------------|------------------------------------|
| Recency    | Days since last purchase            | Lower means more engaged           |
| Frequency  | Number of total purchases           | Higher means more loyal            |
| Monetary   | Total money spent                   | Higher means more valuable         |

### 🔢 Scoring Methodology

- Calculated R, F, M values for each customer.
- Assigned scores from **1 to 5** (quintiles):
  - R → lower days = higher score (most recent)
  - F & M → higher value = higher score
- **RFM Score** = combination of all 3 (e.g., 555, 311, etc.)

---

## 🧠 Customer Segmentation Logic

Based on RFM scores, we define 4 key customer groups:

| Segment            | RFM Traits                                     | Behavior Description                                    | Marketing Strategy |
|--------------------|-----------------------------------------------|----------------------------------------------------------|--------------------|
| ⭐ **High Value**    | R: 4-5, F: 4-5, M: 4-5                         | Very active and high spenders (brand advocates)         | Loyalty rewards, VIP benefits, priority service |
| 💚 **Loyal**        | R: 3-4, F: 3-4, M: 3-4                         | Repeat buyers, good value                              | Cross-sell/Upsell, exclusive bundles |
| ⚠️ **At Risk**       | R: 2-3, F: 1-2, M: 2-3                         | Infrequent buyers who haven't purchased in a while     | Re-engagement emails, limited-time offers |
| 💤 **Dormant**        | R: 1, F: 1, M: 1                              | Stopped buying, likely churned                         | Win-back campaigns, surveys to understand churn |

---

## 📊 Visualizations in Notebook

- Histogram of R, F, M distributions
- RFM Segmentation heatmap
- Customer count by segment
- Revenue contribution by segment
- Top 10 customers by RFM score
- Box plots and line charts for comparison

📍All visualizations are in `Ecommerce_Data_Analysis.ipynb`.

---

## 📊 Power BI Dashboard

📁 `Ecommerce_RFM_Report.pbix` includes:
- Interactive filters for Country, Segment
- RFM distribution charts
- Dynamic customer profiling
- Revenue breakdown per segment

💡 Built for real-time stakeholder demos and marketing team use.

---

## 🧩 Business Strategy Recommendations

| Segment         | Recommendation                                                                 |
|-----------------|----------------------------------------------------------------------------------|
| High Value      | Offer loyalty points, early product access, referral rewards                    |
| Loyal Customers | Promote bundles, cross-sells, and upsells to increase AOV                       |
| At Risk         | Personalized offers, feedback surveys, remarketing ads                          |
| Dormant         | Win-back discount campaigns, conduct NPS or exit-intent surveys                 |

---

## 🧪 How to Run This Project Locally

### 🖥️ Prerequisites
Install Python libraries:

```bash
pip install pandas numpy matplotlib seaborn plotly jupyter
```

### ▶️ Run the Jupyter Notebook
```bash
jupyter notebook Ecommerce_Data_Analysis.ipynb
```

This will perform:
- Data cleaning
- RFM calculation
- Customer segmentation
- Visual analysis
- Strategic insights

---

## 🚀 Future Enhancements
✅ Build a Streamlit App for live customer lookup  
✅ Extend to Customer Lifetime Value (CLTV) prediction  
✅ Automate with Airflow or Scheduled scripts  
✅ Connect to email campaign tools (Mailchimp, Sendinblue)  
✅ Integrate with CRM tools like Salesforce or HubSpot  

---

## 📌 Key Takeaways
- RFM analysis is a powerful segmentation framework with real-world business applications.
- You don't need complex ML to derive high-impact strategies.
- Customer-centric segmentation = Higher revenue + lower churn.

---

## 📬 Contact
Feel free to connect or ask questions:

📧 jinithnaikcareer@gmail.com  
📞 +91-7990554873  
🔗 [LinkedIn – Jinith Naik](https://www.linkedin.com/in/jinithnaik)

---

## 🪪 License
This project is open for educational and portfolio use. Attribution appreciated.

> *"If you don't understand your customer, someone else will."*  
> — Jinith Naik