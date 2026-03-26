# 𝐍 Netflix Content Strategy Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![Made By](https://img.shields.io/badge/Made%20By-Ayush%20Singh-E50914?style=for-the-badge)

---

## 📌 Project Overview

This project simulates a **real-world business intelligence engagement** with Netflix's Content Strategy, Regional Acquisitions, Data Science, and Finance teams. As a Data Analyst, I was approached by a panel of senior stakeholders — including a VP of Content Strategy, Head of Regional Acquisitions, Data Science Lead, and CFO — each with specific, business-critical questions that needed to be answered through data.

The result is a **5-page interactive Power BI dashboard** built on 8,800+ Netflix titles, designed to drive content investment decisions, regional strategy, compliance reviews, and financial projections.

---

## 🏢 Business Context — The Problem

Netflix's leadership team identified several critical gaps in their content visibility:

- 📉 **No unified view** of content distribution across Movies vs TV Shows over time
- 👨‍👩‍👧 **Lack of audience segmentation** — no clarity on what % of catalog is family-friendly vs mature
- 🌍 **Regional blind spots** — leadership couldn't quantify international vs domestic content mix
- 🆕 **No freshness tracking** — subscriber complaints of *"nothing new to watch"* couldn't be validated
- ⚠️ **Compliance risks** — flagged content (NC-17, NR, UR) had no dedicated monitoring view
- 💰 **No investment simulation tool** — CFO had no way to model "what if" scenarios for international content growth

---

## 🎯 Stakeholder Requirements

### 👩‍💼 Sarah Mitchell — VP, Content Strategy
- Movie vs TV Show split trend over time
- Ratings distribution by content type
- Content freshness analysis (2019–2021 vs older)
- Bookmark toggle between Executive and Analyst views

### 🌍 James Okafor — Head of Regional Acquisitions
- Geographic content distribution with country-level drill-down
- Custom hover tooltips showing per-country stats
- Top 10 content-producing countries

### 🧠 Priya Nair — Data Science Lead
- Dynamic `Age Category` calculated column (Classic / Established / Recent / Fresh)
- `Fresh Content %` DAX measure
- What-If parameter for international growth simulation (0–50%)
- Year-over-Year growth % using DAX time intelligence

### 💰 Derek Holt — CFO
- KPI cards with dynamic measures
- Row-Level Security for regional teams
- Cross-report drill-through for flagged content
- Projected content totals using What-If slider

---

## ⭐ STAR Method

### 🔵 Situation
Netflix's content strategy team had 8,800+ titles across 190+ countries but no unified analytical view. Leadership was making content investment decisions based on gut feeling, not data.

### 🟡 Task
Design and deliver a production-grade Power BI dashboard answering 10+ stakeholder questions across content strategy, regional analysis, time intelligence, and compliance — all within a Netflix-branded theme.

### 🟠 Action

- ✅ Performed end-to-end **data cleaning in Power Query** — fixed date formats, extracted `year_added` and `month_added` columns, split duration into value and unit, handled nulls and corrupt rows
- ✅ Built a **DateTable using DAX** and established active/inactive relationships for time intelligence
- ✅ Wrote **23+ DAX measures** including `YoY Growth %`, `Fresh Content %`, `Projected International Titles`, and audience segmentation
- ✅ Implemented a **What-If Parameter** for international content growth simulation (0–50% in 5% increments)
- ✅ Created **Drill-Through pages** enabling right-click genre-level investigation with a Back button
- ✅ Built **Custom Tooltip pages** showing per-country title count, Movie/TV split, and top 3 genres on hover
- ✅ Set up **Bookmarks** for Executive vs Analyst view toggle on Page 1
- ✅ Configured **Row-Level Security** with US Team, India Team, and UK Team regional roles
- ✅ Enabled **Cross-Report Drill-Through** on the Flagged Content compliance page
- ✅ Applied a fully custom **Netflix JSON theme** with dark background (`#141414`), red accents (`#E50914`), and consistent Trebuchet MS typography across all pages

### 🟢 Result

| Metric | Insight |
|---|---|
| Content Mix | 69.6% of catalog is Movies vs 30.4% TV Shows |
| Content Freshness | Only 26.93% of catalog qualifies as "Fresh" (2019–2021) |
| Compliance | US accounts for 43% of all flagged titles |
| International Content | International titles make up 64.68% of the catalog |
| Top Producer | United States produces 3x more content than India |
| Financial Simulation | CFO can now simulate growth scenarios with a live slider |

---

## 📊 Dashboard Pages

| # | Page | Key Visuals & Features |
|---|---|---|
| 1 | **Executive Overview** | 5 KPI Cards, Donut Chart, Bar Chart, Line Chart + YoY, Bookmark Toggle |
| 2 | **Genre Deep-Dive** | Top 10 Genres Bar, Stacked Bar by Type, Audience Breakdown, Drill-Through |
| 3 | **Regional Analysis** | Treemap, Custom Tooltip, Top 10 Countries, Int'l vs Domestic Donut |
| 4 | **Time & Freshness** | YoY Line Chart, Age Category Column, What-If Simulator, Fresh vs Old Donut |
| 5 | **Flagged Content** | Compliance Table, Flagged by Rating, Flagged by Country, RLS |

---

## 🛠️ Power BI Features Used

| Feature | Purpose |
|---|---|
| Power Query | Data Cleaning & Transformation |
| DAX Calculated Columns | Age Category, Audience Type |
| DAX Measures (23+) | KPIs, YoY Growth, Fresh Content %, Projections |
| Time Intelligence | YoY Growth % using DateTable |
| What-If Parameter | International Content Growth Simulator |
| Drill-Through | Genre-level title investigation |
| Custom Tooltip Pages | Per-country hover stats on Treemap |
| Bookmarks | Executive vs Analyst view toggle |
| Row-Level Security | US, India, UK regional data access control |
| Cross-Report Drill-Through | Flagged content compliance navigation |
| Custom JSON Theme | Full Netflix branding across all pages |

---

## 📁 Repository Structure

```
Netflix-Content-Analytics-PowerBI/
│
├── 📊 Netflix_Content_Analytics.pbix    # Power BI Dashboard File
├── 📄 netflix_titles.csv                # Dataset (Source: Kaggle)
├── 🎨 netflix_theme.json                # Custom Power BI Theme File
├── 📸 screenshots/
│   ├── page1_executive_overview.png
│   ├── page2_genre_deepdive.png
│   ├── page3_regional_analysis.png
│   ├── page4_time_freshness.png
│   └── page5_flagged_content.png
└── 📖 README.md
```

---

## 🚀 How to Use This Project

1. **Download** `Netflix_Content_Analytics.pbix` from this repository
2. **Install** Power BI Desktop for free at [powerbi.microsoft.com](https://powerbi.microsoft.com/en-us/desktop/)
3. **Open** the `.pbix` file in Power BI Desktop
4. **Explore** all 5 pages of the dashboard
5. **Try these features:**
   - Right-click any bar in the Genre chart → **Drill Through** → Genre Detail
   - Hover over any country block in the Treemap → **Custom Tooltip** appears
   - Move the **What-If slider** on Page 4 to simulate international growth
   - Click **Executive View / Analyst View** buttons on Page 1 to toggle bookmark views
   - Go to Modeling → View As → Select a role to test **Row-Level Security**

---

## 🖼️ Dashboard Screenshots

### Page 1 — Executive Overview
![Executive Overview](screenshots/page1_executive_overview.png)

### Page 2 — Genre Deep-Dive
![Genre Deep-Dive](screenshots/page2_genre_deepdive.png)

### Page 3 — Regional Analysis
![Regional Analysis](screenshots/page3_regional_analysis.png)

### Page 4 — Time & Freshness
![Time & Freshness](screenshots/page4_time_freshness.png)

### Page 5 — Flagged Content
![Flagged Content](screenshots/page5_flagged_content.png)

---

## 🧮 Key DAX Measures (Sample)

```dax
-- Fresh Content %
Fresh Content % =
DIVIDE(
    CALCULATE(COUNTROWS(netflix_titles), netflix_titles[release_year] >= 2019),
    COUNTROWS(netflix_titles),
    0
) * 100

-- YoY Growth %
YoY Growth % =
DIVIDE(
    ([Total Titles] - [Titles Previous Year]),
    [Titles Previous Year],
    0
) * 100

-- Projected International Titles (What-If)
Projected International Titles =
[International Titles] * (1 + DIVIDE(
    'International Growth %'[International Growth % Value],
    100, 0
))

-- Age Category (Calculated Column)
Age Category =
SWITCH(
    TRUE(),
    netflix_titles[release_year] < 2000, "Classic",
    netflix_titles[release_year] >= 2000 && netflix_titles[release_year] <= 2014, "Established",
    netflix_titles[release_year] >= 2015 && netflix_titles[release_year] <= 2018, "Recent",
    netflix_titles[release_year] >= 2019, "Fresh",
    "Unknown"
)
```

---

## 📄 Dataset Credit & Copyright

> **Dataset:** The Netflix Titles dataset used in this project was sourced from [Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows) and is made available under the public domain.
>
> **Disclaimer:** This project is created purely for **educational and portfolio purposes**. All analysis, DAX measures, data models, visualizations, and business insights are **original work by Ayush Singh** and do not represent official Netflix data or strategy.

---

## 👤 Author

**Ayush Singh**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](your-linkedin-url)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](your-github-url)

---

> ⭐ If you found this project helpful or impressive, please consider giving it a **star** on GitHub!
> It helps others discover the project and motivates me to build more! 🚀
