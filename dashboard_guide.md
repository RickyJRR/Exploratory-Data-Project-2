# 🗺️ Dashboard Navigation Guide

This guide explains how to navigate and interact with the Power BI report.

---

## Requirements
- **Power BI Desktop** (free) — [Download here](https://powerbi.microsoft.com/desktop/)
- No data connection required — the dataset is embedded in the `.pbix` file

---

## Pages

### 1. Define
The starting point. Outlines the initial business questions and scope of the project. Read this first to understand the analytical framework before exploring the data pages.

### 2. Total Sales
The core revenue dashboard. Use the **slicers on the right** to filter all visuals by:
- **Year** — compare 2023, 2024, and 2025
- **Brand** — isolate individual brand performance
- **Sales Channel** — filter by wholesale, distributor, or other channels

Key visuals:
- Top-left card shows **Total Revenue**
- Bar charts show revenue by **brand** and **product category**
- Column charts show **revenue over time** and **% change from 2023**
- Pie chart shows **revenue share by sales channel**

### 3. Redefine
Documents the pivot in analytical direction after Phase 1 findings. Shows the new questions and hypothesis that emerged from the data.

### 4. Marketing
Investigates the relationship between marketing spend and brand performance. Use the **Year** and **Brand** slicers to explore trends.

Key visuals:
- Line charts show **marketing spend over time** by brand and channel
- Column charts show **spend and units sold** by channel
- Stacked charts reveal **channel allocation** differences between brands

### 5. Correlation Page
Tests the hypothesis directly. Use the **Year** and **Sales Channel** slicers to filter the scatter chart.

- Each dot on the scatter chart represents a **brand**
- The **correlation coefficient card** shows the statistical strength of the marketing-revenue relationship
- Look for the **PureLife outlier** — it sits above the trend line on spend but not on revenue

### 6. Narrative (Page 3)
A full written narrative of the project — the thought process, methodology, key findings, and the PureLife anomaly explanation. Best read after exploring the dashboard pages.

---

## Tips
- All visuals on a page are **cross-filtered** — clicking a brand in one chart will filter all other visuals on that page
- Use the **drill-down arrows** on charts with Year/Quarter/Month hierarchy to go from annual to monthly view
- The correlation scatter chart is best explored with the **Sales Channel slicer** to see if the relationship holds within individual channels
