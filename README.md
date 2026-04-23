# E-commerce & Supply Chain Intelligence Dashboard

This Business Intelligence project transforms raw transaction data into a 4-page interactive dashboard to monitor **$10.25M in revenue** and **38,279 orders**. The goal is to provide stakeholders with actionable insights into sales performance, regional dominance, and payment behaviors to optimize supply chain efficiency.

---

## Key Metrics & Business Purpose

| Metric | Value | Business Purpose (The "Why") |
| :--- | :--- | :--- |
| **Total Revenue** | **$10.25M** | Monitor overall financial health and growth scale. |
| **Total Orders** | **38,279** | Track operational load and market demand volume. |
| **Avg. Order Value** | **$267.70** | Understand customer spending power to optimize pricing strategies. |
| **Credit Card Share**| **73.84%** | Assess financial risk and negotiate better rates with payment providers. |
| **Top Region (SP)** | **$4.24M** | Identify the core market to prioritize logistics and marketing budgets. |

---

## Dashboard Architecture

### 1. Executive Overview (KPIs & Trends)
- **Purpose:** Provide an "at-a-glance" status of the business.
- **Insights:** Visualized sales and revenue trends over time, helping management identify seasonal peaks and sudden drops in demand.

### 2. Regional Deep-Dive (Geospatial Analysis)
- **Purpose:** Optimize supply chain and warehouse distribution.
- **Insights:** Mapped revenue by city (Sao Paulo: $1.6M, Rio de Janeiro: $0.8M). This data supports decisions on where to open new distribution centers to reduce shipping times.

### 3. Root-Cause Analysis (Decomposition Tree)
- **Purpose:** Identify the exact drivers behind revenue fluctuations.
- **Insights:** Used AI-driven **Decomposition Trees** to drill down from *State ➔ City ➔ Product Category ➔ Payment Type*. 
- **Discovery:** Revealed that "Toys" in Sao Paulo is a major revenue engine, primarily driven by Credit Card transactions.

### 4. Strategic Insights & Recommendations
- **Purpose:** Translate data into business action.
- **Actionable Advice:** Proposed specific strategies to increase Wallet/Voucher usage to reduce dependency on high-fee credit card payments.

---

## Technical Implementation
- **Data Modeling:** Built a robust **Star Schema** by integrating 5 relational tables (`df_Customers`, `df_Orders`, `df_OrderItems`, `df_Payments`, `df_Products`).
- **ETL Process:** Used **Power Query** for data cleaning, handling missing timestamps, and normalizing currency values.
- **Advanced DAX:** Developed custom measures for AOV (Average Order Value), cumulative revenue, and year-over-year growth.
- **AI Features:** Leveraged **Decomposition Tree** for automated drill-downs and **Q&A** for natural language querying.

---

## Dashboard Preview
*(Insert screenshots of your 4 pages here)*
1. **Overview Page:** ![Overview](Images/page1.png)
2. **Regional Page:** ![Regional](Images/page2.png)
3. **AI Decomposition:** ![AI Tree](Images/page3.png)
4. **Insights Page:** ![Insights](Images/page4.png)

---

## Project Structure
- `Ecommerce_SupplyChain_Analysis.pbix`: Source Power BI file.
- `Data/`: Sample datasets in Kaggle (https://www.kaggle.com/datasets/bytadit/ecommerce-order-dataset) .
