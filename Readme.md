<div align="center">

# 📊 ! Superstore Sales Dashboard ! 📊
### *Interactive Power BI Analytics — Sales, Profit & Order Insights*

[![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Dataset](https://img.shields.io/badge/Dataset-Superstore%20(9%2C994%20Rows)-1F4E79?style=for-the-badge&logo=databricks&logoColor=white)](https://powerbi.microsoft.com/)
[![Visuals](https://img.shields.io/badge/Visuals-Interactive%20%26%20Cross--Filtered-2E7D6B?style=for-the-badge&logo=chartdotjs&logoColor=white)](https://powerbi.microsoft.com/)
[![Pages](https://img.shields.io/badge/Report-2%20Pages-C9A227?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://powerbi.microsoft.com/)
[![Theme](https://img.shields.io/badge/Theme-Executive%20Navy-14213D?style=for-the-badge&logo=figma&logoColor=white)](https://powerbi.microsoft.com/)

<br/>

> *"Data tells a story — a good dashboard lets you click your way through it."*
Video explanation link
https://drive.google.com/file/d/1Why3AuqTbWZhKsUoUQGS9u-6WzlkrRhs/view?usp=sharing
</div>

---

## 📋 Table of Contents

- [📌 Overview](#-overview)
- [🎯 Problem Statement](#-problem-statement)
- [✨ Key Features](#-key-features)
- [🏗️ Project Structure](#️-project-structure)
- [🔄 Project Workflow](#-project-workflow)
- [📈 Part A — Sales Dashboard (Page 1)](#-part-a--sales-dashboard-page-1)
- [🧾 Part B — Order Data (Page 2)](#-part-b--order-data-page-2)
- [🛠️ Tech Stack](#️-tech-stack)
- [📊 Results & Insights](#-results--insights)
- [🏆 Advantages](#-advantages)
- [📄 License](#-license)
- [👤 Author](#-author)
- [🙏 Acknowledgements](#-acknowledgements)

---

## 📌 Overview

The **Superstore Sales Dashboard** is an interactive **Power BI** report that turns nearly **10,000 retail order records** into a clear, clickable story. It combines **KPI cards**, **slicers**, **trend lines**, **bar/column/donut charts** and a **detailed order table**, all connected through **cross-filtering** so that one click updates the whole page.

This project is designed to:
- 📈 Track **Sales, Profit, Quantity and Discount** at a glance
- 🔎 Explore performance by **Region, Segment, Category, Sub-Category, State and Ship Mode**
- 🧭 Drill from **Year → Quarter → Month** on the trend chart
- 🧾 Inspect individual orders on a dedicated, filterable **Order Data** page

---

## 🎯 Problem Statement

> **Objective:** Build an interactive business-intelligence dashboard that helps a retail manager understand *what is selling, where, to whom, and how profitably.*

The report answers questions such as: *Which region earns the most profit? Which sub-categories lose money? How have sales grown year over year? Which customers and orders sit behind the numbers?*

| 📂 Item | 📄 Type | 🔍 Description |
|---------|---------|----------------|
| Superstore | Data Table | 9,994 order lines × 21 columns (2014 – 2017) |
| Dashboard Page | Report Page | KPIs, slicers, 8 charts and a pivot table |
| Order Data Page | Report Page | Slicers, KPIs, order-level table and 2 linked charts |
| Executive Theme | Custom Theme | Navy header with blue / green / gold / red accents |
| Cross-Filtering | Interaction | Click any bar, slice or point to filter the page |

The goal is to demonstrate **practical data-visualisation and dashboard-design skills** in Power BI.

---

## ✨ Key Features

| Feature | Description |
|--------|-------------|
| 🎛️ **5 Slicers per Page** | Region, Segment, Category, Ship Mode and Ship Date dropdowns |
| 💳 **4 KPI Cards** | Total Sales, Total Profit, Total Quantity and Average Discount |
| 📈 **Trend Analysis** | Sales & Profit line chart with Year → Quarter → Month drill-down |
| 🖱️ **Cross-Filtering** | Clicking any visual instantly filters every other visual |
| 🗺️ **Geographic Breakdown** | Sales by State and Profit by Region |
| 🧩 **Product Insights** | Profit by Sub-Category highlights loss-making products |
| 🧾 **Order Explorer** | Full order table with Customer, Product, Quantity and Sales |
| 🎨 **Consistent Design** | Dark navy header, rounded white cards, soft shadows, colour-coded KPIs |

---

## 🏗️ Project Structure

```
📦 superstore-powerbi-dashboard/
│
├── 📄 SuperStoresales-Project.pbix   ← Power BI report (open in Power BI Desktop)
│
└── 📄 README.md                      ← Project documentation
```

---

## 🔄 Project Workflow

```
Superstore Data (9,994 rows)
      │
      ▼
┌─────────────────────────────┐
│   Load into Power BI Model  │  ← Table: Superstore (21 columns)
└────────────┬────────────────┘
             │
     ┌───────┴────────┐
     ▼                ▼
┌─────────────┐   ┌──────────────────┐
│   Page 1    │   │     Page 2       │
│  Dashboard  │   │   Order Data     │
└──────┬──────┘   └────────┬─────────┘
       │                   │
       ▼                   ▼
┌─────────────┐   ┌──────────────────┐
│ Slicers+KPI │   │ Slicers + KPI    │
│ 8 charts +  │   │ Order table +    │
│ pivot table │   │ donut + bar      │
└──────┬──────┘   └────────┬─────────┘
       │                   │
       ▼                   ▼
┌─────────────────────────────┐
│   Click / Filter / Drill    │
└────────────┬────────────────┘
             │
             ▼
   All visuals update together ✅
```

---

## 📈 Part A — Sales Dashboard (Page 1)

### 🎛️ 1. Filters & KPIs

The top of the page holds five dropdown slicers and four colour-coded KPI cards.

| KPI Card | Field | Aggregation | Colour |
|----------|-------|-------------|--------|
| 💰 **Sales** | `Sales` | Sum | ![#1F4E79](https://img.shields.io/badge/-1F4E79-1F4E79?style=flat-square) Blue |
| 📈 **Profit** | `Profit` | Sum | ![#2E7D6B](https://img.shields.io/badge/-2E7D6B-2E7D6B?style=flat-square) Green |
| 📦 **Quantity** | `Quantity` | Sum | ![#C9A227](https://img.shields.io/badge/-C9A227-C9A227?style=flat-square) Gold |
| 🏷️ **Discount** | `Discount` | Average | ![#B5483F](https://img.shields.io/badge/-B5483F-B5483F?style=flat-square) Red |

---

### 🗺️ 2. Visuals — Overview

| # | Visual | Type | Fields Used |
|---|--------|------|-------------|
| 1️⃣ | **Sales & Profit Trend** | Line Chart | Order Date (Year/Quarter/Month), Sales, Profit |
| 2️⃣ | **Category: Sales vs Profit** | Clustered Column | Category, Sales, Profit |
| 3️⃣ | **Sales by Segment** | Donut Chart | Segment, Sales |
| 4️⃣ | **Profit by Region** | Clustered Bar | Region, Profit |
| 5️⃣ | **Total Revenue by Product Category** | Clustered Bar | Category, Region, Sales |
| 6️⃣ | **Profit by Sub-Category** | Clustered Bar | Sub-Category, Profit |
| 7️⃣ | **Sales by State** | Clustered Bar | State, Sales |
| 8️⃣ | **Order Summary** | Pivot Table | Category, Sub-Category, Customer Name, Order ID, Sales, Profit |

---

### 📉 3. Trend Analysis

> Monthly / quarterly / yearly view of **Sales** and **Profit** together.

**How to use it:**
```
Click a point        → filters the whole page to that period
Use the drill arrows → Year ➜ Quarter ➜ Month
```

---

### 🧩 4. Category, Segment & Region Charts

> Compare performance across business dimensions and spot weak areas quickly.

```
Click "Technology"   → every visual shows Technology only
Click "Consumer"     → every visual shows the Consumer segment only
Click "West"         → every visual shows the West region only
Click again          → clears the filter
```

---

## 🧾 Part B — Order Data (Page 2)

### 🔍 5. Order Explorer

> A detailed, order-level view that reacts to every slicer and chart.

**Page layout:**

| Area | Content |
|------|---------|
| 🔝 **Top** | Dark header + Region, Segment, Category, Ship Mode and Ship Date slicers |
| 💳 **Below filters** | Sales, Profit, Quantity and Discount KPI cards |
| 📋 **Left (large)** | Order table — Customer Name, Order Date, Order ID, Product Name, Quantity, Sales |
| 🍩 **Right (top)** | Sales by Segment donut — click a slice to filter the table |
| 📊 **Right (bottom)** | Sales & Profit by Category — click a bar to filter the table |

**Key Concepts Used:**

| Concept | Detail |
|---------|--------|
| 🎛️ **Slicers** | Dropdown filters shared by all visuals on the page |
| 🖱️ **Cross-Filtering** | Charts filter the table (and the KPI cards) on click |
| 📅 **Date Hierarchy** | Auto date hierarchy on Order Date and Ship Date |
| 🎨 **Custom Theme** | `Executive` theme on top of the Fluent 2 base theme |

---

## 🛠️ Tech Stack

| Tool | Version | Purpose |
|------|---------|---------|
| 📊 **Power BI Desktop** | Latest | Report authoring and visualisation |
| 🗃️ **Power BI Data Model** | Built-in | Superstore table with 21 columns |
| 📈 **Native Visuals** | Built-in | Cards, slicers, line, bar, column, donut, pivot table, table |
| 📅 **Auto Date/Time** | Built-in | Year → Quarter → Month hierarchy |
| 🎨 **Custom Theme** | JSON | Executive colour palette |

**Colour Palette**

![#14213D](https://img.shields.io/badge/Header-14213D-14213D?style=for-the-badge)
![#1F4E79](https://img.shields.io/badge/Sales-1F4E79-1F4E79?style=for-the-badge)
![#2E7D6B](https://img.shields.io/badge/Profit-2E7D6B-2E7D6B?style=for-the-badge)
![#C9A227](https://img.shields.io/badge/Quantity-C9A227-C9A227?style=for-the-badge)
![#B5483F](https://img.shields.io/badge/Discount-B5483F-B5483F?style=for-the-badge)
![#F3F5F8](https://img.shields.io/badge/Background-F3F5F8-F3F5F8?style=for-the-badge&labelColor=555)

---

## 📊 Results & Insights

**Dataset at a glance (2014 – 2017)**

| 📌 Metric | 🔢 Value |
|-----------|----------|
| 💰 Total Sales | **$2.30 M** |
| 📈 Total Profit | **$286 K** (≈ 12.5 % margin) |
| 📦 Total Quantity Sold | **37,873 units** |
| 🏷️ Average Discount | **15.6 %** |
| 🧾 Unique Orders | **5,009** |
| 👥 Customers / Products | **793 / 1,862** |
| 🗺️ States / Cities | **49 / 531** |

**What the dashboard reveals**

- ✅ **Sales are growing** — from about $484 K in 2014 to $733 K in 2017 (roughly **+51 %**), with a small dip in 2015.
- 💻 **Technology leads** — highest sales ($836 K) and profit ($145 K).
- 🪑 **Furniture is the weak spot** — $742 K in sales but only $18 K in profit (≈ 2.5 % margin).
- 🌎 **West is the top region** — $725 K sales and $108 K profit; **South** is the smallest.
- 👤 **Consumer segment** brings in about **51 %** of total sales.
- 🚚 **Standard Class** shipping accounts for roughly **59 %** of sales.
- 🔻 **Loss-making sub-categories** — Tables (≈ –$17.7 K), Bookcases (≈ –$3.5 K) and Supplies (≈ –$1.2 K).
- 🏅 **Most profitable sub-categories** — Copiers, Phones and Accessories.

---

## 🏆 Advantages

| Advantage | Detail |
|-----------|--------|
| 🎓 **Beginner Friendly** | Uses only built-in Power BI visuals — no custom code needed |
| 🖱️ **Highly Interactive** | One click filters the entire page |
| 📚 **Educational** | Shows slicers, KPIs, drill-down and cross-filtering in one report |
| 🎨 **Clean Design** | Consistent colours, rounded cards and clear titles |
| ⚡ **Fast to Explore** | KPIs, trends and details are all visible without scrolling |
| 🧪 **Extensible** | Easy to add DAX measures (Profit Margin, YoY Growth), maps or bookmarks |
| 🧾 **Detail on Demand** | Dedicated Order Data page for row-level checks |
| 🛡️ **Self-Contained** | Single `.pbix` file with the data embedded |

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for full details.

```
MIT License — Free to use, modify, and distribute with attribution.
```

---

## 👤 Author

<div align="center">

Asvi Ambaliya

[![GitHub](https://img.shields.io/badge/GitHub-yourhandle-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/yourhandle)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yourprofile/)

> *"Every great decision starts with a single chart."*

**🎓 Role:** Data Analyst | Power BI Enthusiast \
**📍 Location:** India\
**🛠️ Skills:** Power BI · Data Visualisation · Dashboard Design · Data Storytelling

</div>

---

## 🙏 Acknowledgements

Special thanks to the following resources and communities that made this project possible:

- 📚 [Microsoft Power BI Docs](https://learn.microsoft.com/power-bi/) — Official Power BI documentation
- 📊 [Power BI Visuals Guide](https://learn.microsoft.com/power-bi/visuals/power-bi-visualization-types-for-reports-and-q-and-a) — Visualisation types reference
- 🛒 [Superstore Dataset](https://www.kaggle.com/) — Popular retail sample dataset
- 🎨 [Coolors](https://coolors.co/) — Colour palette inspiration
- 💬 [Power BI Community](https://community.fabric.microsoft.com/) — Problem-solving support
- 📖 [Microsoft Learn](https://learn.microsoft.com/training/powerplatform/power-bi) — Power BI learning paths

---

<div align="center">
Asvi Ambaliya
</div>
