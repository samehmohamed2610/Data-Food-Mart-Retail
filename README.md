# 🛒 Food Mart — Retail Analysis Dashboard

A multi-page interactive Power BI solution providing a 360° view of retail performance across sales, customers, and products.

**Developed by:** [Sameh Elaraby](https://github.com/samehmohamed2610)

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=flat)
![Power Query](https://img.shields.io/badge/Power%20Query-217346?style=flat)
![Star Schema](https://img.shields.io/badge/Star%20Schema-5C2D91?style=flat)

---

## 📌 Overview

Food Mart operates 24 stores across multiple regions, selling 1,560 products to roughly 8,800 unique customers. This report consolidates sales, returns, customer, and product data into a single star-schema model so the business can see where revenue comes from, which customers and brands drive it, and where returns eat into it.

Data was cleaned and shaped in Power Query, modeled as a star schema in Power BI, and all metrics calculated in DAX.

---

## 📈 Headline Numbers

| Metric | Value |
| --- | --- |
| Total sales | $1.76M |
| Net sales | $1.75M |
| Gross profit | $1.05M |
| Profit margin | 59.70% |
| Total returns | $17.43K |
| Unique customers | 8,842 |
| Avg. spend per customer | $171.60 |
| Avg. order value | $6.54 |
| Total quantity sold | 833.5K units |
| Products | 1,560 |

---

## 🖥️ Report Pages

### 📊 Overview Page

Tracks overall business health through five core KPIs: total sales, gross profit, profit margin, total returns, and net sales.

- **Sales and profit by month** — seasonal trend across all twelve months, peaking at $177K in December.
- **Top 20 brands** — Hermanos leads at $57K, followed by Tell Tale and Ebony.
- **Sales by region** — North West dominates at $847.83K, ahead of Mexico Central ($330.36K) and South West ($320.80K).
- **Customer-level table** — sales amount, quantity, gross profit, and return amount per customer.

![Overview Page](screenshots/0.png)

### 👥 Customers Page

Focuses on customer behavior through total customers (10.28K), unique customers (8,842), average spend, average order value, and customer frequency (673).

| Member card tier | Share of sales |
| --- | --- |
| Bronze | 55.91% |
| Normal | 23.06% |
| Golden | 12.68% |
| Silver | 8.36% |

- **Sales by gender** — female $851.73K against male $872.82K, an almost even split.
- **Top customers by profit** — led by Ida Rodriguez at $1.34K.
- **Returns by month** — a clear spike across November and December, reaching 1.72K.

![Customers Page](screenshots/1.png)

### 📦 Products Page

Covers product-level performance through total quantity, average price ($2.12), total cost ($711.7K), total returns (8,289 units), and product count.

- **Returns vs quantity by month** — combo chart overlaying return volume against units sold.
- **Quantity by brand** — 18 brands ranked, with Hermanos leading at 24.7K units.
- **Store comparison** — sales and gross profit across all 24 locations, with Store 13 topping at $170.40K.
- **Product detail table** — sales, quantity, gross profit, and returns per product.

![Products Page](screenshots/2.png)

### 🔍 Decomposition Tree

Interactive drill-down of the full $1,764,546.44 in total sales, broken down hierarchically by product name and then by store city, with profit margin, average spend, total returns, and average order value shown alongside.

This page supports root-cause analysis: it isolates which specific products and locations drive or drag overall performance rather than showing aggregates alone.

![Decomposition Tree](screenshots/3.png)

### 🎛️ Global Filters

Every page carries a Month Name dropdown and a Quarter toggle (1–4), applied simultaneously across all visuals for consistent time-based filtering.

![Global Filters](screenshots/4.png)

---

## 💡 Key Takeaways

**01 · Revenue is regionally concentrated** — North West alone accounts for roughly 48% of total sales, more than the next two regions combined. This is a strength and a risk worth monitoring.

**02 · Bronze tier carries the business** — 55.91% of sales come from the lowest loyalty tier, which suggests the upper tiers are either too small or not delivering enough incentive to upgrade.

**03 · Returns are seasonal** — the November–December spike coincides with peak sales, so return handling capacity should scale with the holiday period rather than stay flat.

**04 · Small baskets, repeat visits** — a $6.54 average order value against $171.60 average customer spend means customers return often. Frequency, not basket size, is the growth lever.

**05 · Store performance varies widely** — Store 13 at $170.40K sits well above the roughly $73K average across 24 stores, making it a useful benchmark for the weaker locations.

---

## 🛠️ Tools and Technologies

| Tool | Purpose |
| --- | --- |
| Power Query | Data cleansing, shaping, and transformation |
| Power BI | Star-schema data modeling and report design |
| DAX | KPIs, margin, returns, and customer measures |
| Slicers & Bookmarks | Month and quarter filtering across pages |
| Decomposition Tree | Hierarchical drill-down analysis |

---

## 📁 Repository Structure

```
Food-Mart-Retail-Analysis/
├── data/                        # Raw and cleaned dataset
├── screenshots/                 # Dashboard page exports
├── Food_Mart_Retail_Analysis.pbix
└── README.md
```

---

## ▶️ How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/samehmohamed2610/Food-Mart-Retail-Analysis.git
   ```
2. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free).
3. Open the `.pbix` file.
4. If the data source path differs on your machine, update it under **Transform data → Data source settings**, then refresh.

---

## 👤 Author

**Sameh Elaraby**
GitHub: [@samehmohamed2610](https://github.com/samehmohamed2610)

If this project was useful to you, consider giving the repository a ⭐.
