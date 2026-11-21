# Datheon Data Analytics & Power BI Internship

- **Program:** Data Analytics & Power BI Internship — Datheon
- **Application ID:** `DT-2026-O5P11`
- **Participant:** Raditya

---

## Task Progress

| Task | Title | Status | Folder |
| :--- | :--- | :---: | :--- |
| **Task 1** | Exploratory Data Analysis (EDA) on Superstore Retail Sales | ✅ Completed | [`Task_1_Superstore_EDA/`](./Task_1_Superstore_EDA) |
| **Task 2** | Power BI Executive Dashboard | 🔄 In Progress | [`Task_2_PowerBI_Executive_Dashboard/`](./Task_2_PowerBI_Executive_Dashboard) |

---

## Tools & Tech Stack
- **Data Analysis & Wrangling:** Python 3, Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Notebooks:** Jupyter Notebook / Google Colab
- **BI & Reporting (Task 2):** Power BI Desktop, DAX

---

## Repository Structure

```text
Datheon_Data_Analytics_-_Power_BI_Internship/
├── README.md
├── requirements.txt
├── .gitignore
├── Task_1_Superstore_EDA/
│   ├── data/
│   │   └── superstore_sales.csv
│   ├── outputs/
│   │   ├── 01_customer_volume_and_segment.png
│   │   ├── 02_monthly_seasonality_and_velocity.png
│   │   ├── 03_category_subcategory_region_profit.png
│   │   └── 04_discount_sensitivity_and_margin.png
│   └── DATHEON_TASK_1.ipynb
└── Task_2_PowerBI_Executive_Dashboard/
    ├── README.md
    └── screenshots/
```

---

## Task 1 — Key Executive Takeaways (Superstore Retail Sales)

From **9,993** cleaned line items (**5,009** unique orders, **793** unique customers, **$2,296,919.49** total sales, **$286,409.08** total profit, **12.47%** overall margin across 2015–2018):

1. **The 20% Discount Cliff (`Discount > 20%` Destroys $135K in Profit):**
   Orders with 0%–20% discounts (86.1% of line items) generated **$1,934,430.71** in sales and **$421,773.08** in profit (**21.80% margin**). Every discount tier above 20% (`30%–80%`, 13.9% of line items) was net unprofitable, generating $362,488.78 in sales while losing **-$135,364.00 (-37.34% margin)** with a 96.8% loss rate ($r = -0.864$ between Discount and Profit Margin).
2. **Technology & Office Supplies Drive 93.6% of Profit While Furniture Bleeds Margin:**
   **Technology** ($145,454.95 profit, 17.40% margin) and **Office Supplies** ($122,490.80 profit, 17.04% margin) deliver **93.55%** of total profit. **Furniture** yields only $18,463.33 (**2.49% margin**) due to heavy losses in **Tables** (-$17,725.48, -8.56% margin) and **Bookcases** (-$3,472.56, -3.02% margin).
3. **Strong Q4 Seasonality (51.6% of Revenue in Sep–Dec) & Accelerating YoY Growth:**
   Annual revenue grew **+51.5%** from 2015 ($483,966) to 2018 ($733,215). **September–December** drives **51.62%** of total revenue, and **Q4 (Oct–Dec)** alone drives **38.23%**. Peak months **November ($352,461)** and **December ($325,294)** generate nearly **6×** February's trough ($59,751).
4. **Central Region Margin Leakage (7.92% vs. West's 14.94%):**
   **West** leads in profit ($108,418) and margin (**14.94%**) with disciplined discounting (10.9% avg). **Central** generates 28% more revenue than South ($501,240 vs. $391,722) yet delivers the lowest profit ($39,706, **7.92% margin**) due to an average discount of **24.0%**.
5. **High Customer Retention (98.5% Repeat Rate) With B2B Margin Upside:**
   **98.49%** of customers (781/793) placed 2+ orders (mean **6.32 orders**, **$2,896.49** lifetime spend). **Consumer** brings 50.56% of revenue at an 11.55% margin ($449.11 AOV), while **Home Office** (14.05% margin, $472.36 AOV) and **Corporate** (13.03% margin, $466.41 AOV) deliver stronger unit economics.
