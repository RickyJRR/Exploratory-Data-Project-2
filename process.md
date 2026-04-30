# 📝 Analytical Process

This document walks through the full thought process behind the FMCG Sales & Marketing Power BI project — from first look at the data to final conclusions.

---

## Step 1 — Data Familiarization (Before Any Analysis)

After acquiring the dataset, the first instinct was to dive straight into building visuals. Instead, I opened the data in **Power BI's Table View** to understand what I was working with before touching anything.

The dataset was relatively clean but wide — containing many attributes (columns) across a multi-year span. This preliminary step was critical. Without understanding the shape and content of the data first, analysis risks being directionless.

> **Principle applied:** Messy Data IN = Messy Analysis OUT.

---

## Step 2 — Define the Scope (Phase 1)

With a large dataset and many possible directions, I defined a focused set of initial questions to give the analysis structure and intention:

- What products generate the most revenue?
- How does revenue break down over time?
- Which brands and product categories are top performers?
- How does the sales channel affect revenue?

I narrowed the focus further to **Financial Performance and Top-Line Growth**, making **Net Revenue (USD)** the primary metric.

---

## Step 3 — Build the Total Sales Dashboard

To answer Phase 1 questions, I built the following visuals on the **Total Sales** page:

- **KPI Card** — Total Revenue across the entire dataset
- **Clustered Bar Charts** — Revenue by brand and by product category, with year/quarter/month drill-down
- **Pie Chart** — Revenue share by sales channel
- **Column Charts** — Revenue change over time and % difference from 2023 baseline
- **Slicers** — Year, brand, and sales channel for interactivity

---

## Step 4 — Surface Insights and Redefine (Phase 2)

From the Total Sales visuals, one key finding stood out immediately:

**Total revenue increased by $422,972.83 (9.21%)** from 2023 to 2025.

But when broken down by brand, the picture became more interesting — and more questions emerged:

- **HomeNest**, the 4th highest-earning brand in 2023, became the **#1 brand by 2025**
- **FuelCore** and **RoastTrail**, the top 2 earners in 2023, dropped to 3rd and 5th place respectively

This prompted a redefine of the project's direction:

> **New hypothesis:** The shifts in brand revenue rankings are related to changes in marketing spend.

---

## Step 5 — Marketing Spend Analysis

To investigate the hypothesis, I built the **Marketing** page:

- **Line Charts** — Marketing spend over time by brand and by sales channel
- **Clustered Column Chart** — Marketing spend by sales channel
- **100% Stacked Column Charts** — Marketing spend and revenue share by brand and channel
- **Units Sold** — Bar chart showing average units sold per sales channel

**Findings:**
- HomeNest showed a clear **increase in marketing spend** over the period
- FuelCore and RoastTrail showed **decreasing marketing investment**
- Wholesale was the dominant sales channel by units sold (507 avg vs. 325 for distributor)

These trends visually aligned with the revenue shifts — but I wanted to quantify the relationship.

---

## Step 6 — Correlation Analysis

To test the hypothesis formally, I built the **Correlation Page**:

- **Scatter Chart** — Marketing Spend (Y) vs. Net Revenue (X), plotted by brand
- **Correlation Coefficient Card** — Showing the statistical strength of the relationship

**Result:** A **strong positive correlation** was confirmed between marketing spend and revenue.

---

## Step 7 — The PureLife Anomaly

One brand broke the pattern: **PureLife** had the highest total marketing spend but did **not** have the highest revenue.

Investigating channel allocation revealed the reason:

| Brand | % Marketing Spend in Wholesale |
|-------|-------------------------------|
| PureLife | 24.8% |
| HomeNest | 29.5% |

PureLife's underallocation to the wholesale channel — the highest-volume channel — explains why high spend didn't translate to high revenue. **It's not just how much you spend, it's where you spend it.**

---

## Conclusion

This project demonstrates a complete analytical workflow:

1. Data familiarization before analysis
2. Scoped initial questions (Define)
3. Built visuals to answer those questions
4. Let the data generate new questions (Redefine)
5. Formed and tested a hypothesis
6. Identified and explained an anomaly

The result is a multi-page, interactive Power BI report that tells a complete data story — from top-line revenue performance to a channel-level marketing efficiency insight.
