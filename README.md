# 🛒 Ecommerce Sales Dashboard

> A fully interactive sales analytics dashboard — zero frameworks, zero backend, 100% in-browser.

**[🔴 Live Demo →](https://pallab-chakraborty.github.io/ecommerce-dashboard/)**

![Ecommerce Sales Dashboard Preview](https://pallab-chakraborty.github.io/ecommerce-dashboard/preview.png)

---

## 📌 About the Project

This dashboard visualizes **1,500 order lines** from an Indian e-commerce business across the full year of 2018, spanning **500 unique customers** across 3 product categories and 5 payment modes.

Built entirely in a **single HTML file** — no React, no Node, no build step. The raw CSV data (`Orders.csv` + `Details.csv`) was cleaned, merged on `Order ID`, aggregated, and embedded directly into the HTML. Every chart and table updates live when filters are applied.

| Metric | Value |
|---|---|
| 💰 Total Revenue | ₹4,37,771 |
| 📈 Net Profit | ₹36,963 |
| 📦 Units Sold | 5,615 |
| 🛍️ Avg Order Value | ₹292 |
| 👥 Customers | 500 |
| 📋 Order Lines | 1,500 |
| 📊 Profit Margin | 8.4% |

---

## ✨ Features

- **Dynamic Filters** — filter by Category (Electronics / Furniture / Clothing) and Payment Mode (COD / UPI / Credit Card / EMI / Debit Card); all 8 charts and tables re-render instantly
- **Monthly Trend Line** — revenue vs profit across all 12 months of 2018, revealing seasonal dips and peaks
- **Payment Mode Donut** — visual breakdown of how customers prefer to pay
- **Category Bar Chart** — grouped revenue & profit comparison across the 3 categories
- **Top States by Revenue** — animated bar list for geographic sales distribution (Maharashtra leads at ₹1,02,498)
- **Sub-Category Profit Table** — profit/loss drilldown to product-type level (e.g. Printers: +₹8,606 vs Electronic Games: -₹644)
- **Top 10 Customers** — ranked by total lifetime spend with 🥇🥈🥉 medals
- **Revenue vs Quantity Chart** — side-by-side comparison to spot high-volume, low-revenue categories

---

## 🛠️ Tech Stack

| Tool | Role |
|---|---|
| HTML5 + CSS3 | Layout, theming, animations |
| Vanilla JavaScript (ES6+) | Data joins, aggregations, filter logic |
| [Chart.js 4.4](https://www.chartjs.org/) | All 5 interactive charts |
| Google Fonts — Outfit + JetBrains Mono | Typography |
| GitHub Pages | Free static hosting |

> **No npm. No bundler. No dependencies beyond a CDN link.** The entire app is a single `index.html` — open it in any browser and it works.

---

## 📁 Data Sources

| File | Rows | Key Columns |
|---|---|---|
| `Orders.csv` | 500 | Order ID, Order Date, CustomerName, State, City |
| `Details.csv` | 1,500 | Order ID, Amount, Profit, Quantity, Category, Sub-Category, PaymentMode |

The two tables are joined on `Order ID` at build time, and the merged JSON (1,500 records) is embedded inline in the HTML so the dashboard runs with zero API calls.

---

## 🚀 Run Locally

```bash
git clone https://github.com/pallab-chakraborty/ecommerce-dashboard.git
cd ecommerce-dashboard

# Just open the file — no server needed
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

---

## 🔗 Related Projects

| Project | Description | Live |
|---|---|---|
| 🚲 Bike Sales Dashboard | Customer segmentation & purchase behavior — 1,000 records, interactive filters | [Live Demo](https://pallab-chakraborty.github.io/bike-sales-dashboard/) |
| 🌐 Personal Portfolio | My full developer portfolio | [Visit](https://pallab-chakraborty.github.io/pallab/) |

---

## 👤 Author

**Pallab Chakraborty**
B.Tech CSE · Jawaharlal Nehru University, New Delhi

[![Portfolio](https://img.shields.io/badge/Portfolio-pallab--chakraborty.github.io-blueviolet?style=flat-square)](https://pallab-chakraborty.github.io/pallab/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pallabchakrabortyjnu-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/pallabchakrabortyjnu/)
[![GitHub](https://img.shields.io/badge/GitHub-Pallab--Chakraborty-black?style=flat-square&logo=github)](https://github.com/Pallab-Chakraborty)
[![Email](https://img.shields.io/badge/Email-pallab98__soe@jnu.ac.in-red?style=flat-square&logo=gmail)](mailto:pallab98_soe@jnu.ac.in)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<p align="center">Built with ❤️ & ☕ by <a href="https://pallab-chakraborty.github.io/pallab/">Pallab Chakraborty</a></p>
