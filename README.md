# 🛒 Retail Sales Data Analysis

A Python-based data analysis project that cleans raw retail transaction data, uncovers sales trends, and generates a visual, easy-to-read HTML report — built to handle real-world messy data, not just a tidy sample dataset.

---

## 📌 What This Project Does

Retail sales data usually comes with gaps — missing prices, missing quantities, inconsistent discount flags. Instead of dropping every incomplete row, this pipeline tries to **recover** what it can before falling back to removing truly unusable records, then turns the cleaned data into a full sales analysis.

**Pipeline steps:**

`Load CSV → Validate Columns → Clean & Reconstruct → Analyze → Visualize → Generate HTML Report`

---

## 🔍 Key Analysis Areas

| Area | What It Shows |
|---|---|
| Revenue Trend | Monthly and yearly revenue movement |
| Category Performance | Which product categories drive the most (and least) revenue |
| Channel Behavior | Online vs. in-store sales split |
| Payment Methods | Distribution of how customers pay |
| Discount Impact | Whether discounts actually increase average order value |
| Customer Insights | Top spenders and revenue concentration |
| Transaction Distribution | Spread and skew of individual purchase amounts |

---

## 🛠️ Tech Stack

- **Python** — core logic
- **pandas** — data cleaning & aggregation
- **matplotlib** — chart generation
- **HTML/CSS** — final report layout (auto-generated, no manual editing needed)

---

## 📂 What You Get After Running It

```
retail_sales_cleaned.csv        →  cleaned, analysis-ready dataset
charts/                         →  7 PNG charts
retail_sales_analysis.html      →  final report, opens in any browser
```

---

## ▶️ How to Run

```bash
pip install pandas numpy matplotlib
python retail_sales_analysis.py
```

Then open `retail_sales_analysis.html` in your browser.

> Update the `INPUT_CSV` variable at the top of the script to point to your own file.

---

## 📋 Required Columns

```
Transaction Date, Price Per Unit, Quantity, Total Spent,
Category, Item, Payment Method, Location, Customer ID, Discount Applied
```

If a column is missing, the script stops immediately and tells you exactly what's missing — instead of crashing halfway through the analysis.

---

## 💡 What Makes This Different

Most beginner data projects assume the dataset is already perfect. This one is built the way real analysis actually starts: messy data, missing values, and schema surprises — handled with recovery logic and validation instead of guesswork.

---

## 📄 License

MIT — free to use, modify, and build on.
