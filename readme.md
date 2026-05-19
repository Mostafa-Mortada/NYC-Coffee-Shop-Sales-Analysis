<div align="center">
  
#  NYC Coffee Shop | Sales Analysis

![Tool](https://img.shields.io/badge/Tool-Microsoft%20Excel-217346?style=flat-square&logo=microsoft-excel&logoColor=white)
![Domain](https://img.shields.io/badge/Domain-Retail%20%26%20Sales-brown?style=flat-square)
![Locations](https://img.shields.io/badge/Locations-3%20NYC%20Stores-blue?style=flat-square)
![Transactions](https://img.shields.io/badge/Transactions-149%2C116-orange?style=flat-square)

A data analysis project exploring coffee sales performance across **three NYC locations**: Astoria, Hell's Kitchen, and Lower Manhattan covering 6 months of transactional data.
<div>
---

## 🗺️ Locations

- 🏙️ Astoria
- 🍳 Hell's Kitchen
- 🗽 Lower Manhattan

---

## 📊 Highlights

| Metric | Value |
|---|---|
| 💰 Total Revenue | $698,812 |
| 🧾 Total Transactions | 149,116 |
| 💵 Revenue Per Transaction | $4.69 |
| 📦 Units Per Transaction | 1.44 |

---

## 🗃️ Dataset

### Original Columns

| Column | Description |
|---|---|
| `transaction_id` | Unique identifier for each transaction |
| `transaction_date` | Date the transaction occurred |
| `transaction_time` | Time the transaction occurred |
| `transaction_qty` | Number of units purchased |
| `store_id` | Unique identifier for the store |
| `store_location` | Store location name |
| `product_id` | Unique identifier for the product |
| `unit_price` | Price per unit |
| `product_category` | High-level product category (e.g. Coffee, Tea, Bakery) |
| `product_type` | Product type within the category |
| `product_detail` | Specific product name |

### 🔧 Feature Engineering

Four new columns were added to support time-based and revenue analysis:

| Column | Description |
|---|---|
| `Revenue` | Calculated as `transaction_qty × unit_price` |
| `Month` | Extracted from `transaction_date` |
| `Day_of_week` | Extracted from `transaction_date` |
| `Hour` | Extracted from `transaction_time` |

### 🧹 Data Cleaning

- Removed duplicate records
- Handled null values

---

## 💡 Key Insights

- **Revenue more than doubled** from January ($81K) to June ($166K) — a 103% growth over 6 months
- **Morning rush is everything** — peak hours are 8 AM to 10 AM, driving over half of daily transactions
- **Coffee & Tea dominate** — together accounting for ~69% of all transactions (58K and 45K respectively)
- **Barista Espresso** is the top revenue-generating product at $91,406
- **Brewed Chai Tea** leads in transaction volume with 17,183 orders
- **Weekends are slightly slower** — Saturday has the lowest traffic of the week, a potential opportunity for targeted promotions
- **Bakery is a strong side category** — 22K+ transactions show solid food attachment alongside drinks

---

## 🏆 Top Products

| Product | Category | Revenue |
|---|---|---|
| Barista Espresso | Coffee | $91,406 |
| Brewed Chai Tea | Tea | $77,082 |
| Hot Chocolate | Drinking Chocolate | $72,416 |
| Gourmet Brewed Coffee | Coffee | $70,035 |
| Brewed Black Tea | Tea | $47,932 |

---

## 🛠️ Tools Used

- **Microsoft Excel** — Data cleaning, Pivot Tables, and Dashboard
- **Excel Slicers** — Interactive filtering by location

---

## 📁 Project Structure

```
coffee-sales-analysis/
│
├── data/
│   └── coffee_sales_raw.xlsx
│
├── analysis/
│   └── coffee_sales_analysis.xlsx
│
├── dashboard/
│   └── Dashboard.png
│
└── README.md
```

---

*Data covers January – June | All 3 locations combined*
