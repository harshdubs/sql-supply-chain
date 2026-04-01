# 📦 Supply Chain Business Insights — SQL Analysis

A deep-dive SQL analysis project on a 500K+ row supply chain dataset, uncovering cost drivers, supplier performance issues, and inventory inefficiencies — presented as both a technical notebook and an executive-ready dashboard.

---

## 📌 What this project does

Supply chain data is often sitting in databases untouched, full of insight that operations and finance teams never see. This project treats it like a real business problem:

- **Who are our worst-performing suppliers and why?**
- **Where is inventory piling up, and what's it costing us?**
- **Which product categories have the longest delays?**

All answered entirely in SQL, then visualised in Excel for stakeholder delivery.

---

## 🔍 SQL Techniques Used

| Technique | Applied To |
|-----------|-----------|
| CTEs (Common Table Expressions) | Multi-step calculations, readable query structure |
| Window Functions — RANK() | Ranking suppliers by delay frequency |
| Window Functions — LAG(), LEAD() | Month-over-month delay trend comparison |
| Window Functions — Running SUM() | Cumulative cost tracking over time |
| Multi-table JOINs | Linking orders, suppliers, products, inventory |
| CASE statements | Categorising delay severity |
| Subqueries | Filtering aggregated results |

---

## 📊 Key Insights Found

- **Top 3 suppliers** accounted for 62% of all delayed orders
- **Electronics category** had 2.3x the average delay vs other categories
- Inventory turnover in the **South region** was 40% lower than North — excess stock worth ₹2.1Cr sitting idle
- Month-over-month analysis revealed delays spike in **Q4** consistently — pointing to a seasonal planning gap

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| SQL Server | Primary analysis environment |
| Python (Pandas) | Data loading, validation, supplementary EDA |
| Excel | Executive dashboard (pivot tables, conditional formatting) |
| Jupyter Notebook | Full documented analysis walkthrough |

---

## 📁 Project Structure

```
sql-supply-chain/
│
├── data/
│   └── supply_chain_sample.csv
│
├── sql/
│   └── 01_supplier_performance.sql
│   └── 02_inventory_analysis.sql
│   └── 03_delay_trends.sql
│   └── 04_cost_drivers.sql
│
├── notebooks/
│   └── full_analysis_walkthrough.ipynb
│
├── dashboard/
│   └── supply_chain_insights.xlsx
│
└── README.md
```

---

## 🚀 How to run

```bash
git clone https://github.com/cosmicskull711/sql-supply-chain
cd sql-supply-chain
# Load supply_chain_sample.csv into SQL Server or SQLite
# Run SQL files in order (01 → 04)
# Open notebook for full walkthrough
jupyter notebook notebooks/full_analysis_walkthrough.ipynb
```

---

## 👤 Author

**Harsh Dubey** — [LinkedIn](https://www.linkedin.com/in/harsh-dubey-1b169a242) · [GitHub](https://github.com/cosmicskull711)
