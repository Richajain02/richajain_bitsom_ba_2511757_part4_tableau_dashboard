# Chart Selection Justification

## Overview

This document explains the chart selection and visualization design principles used in the Executive Sales Performance Dashboard. The dashboard follows best practices for data visualization by using appropriate chart types, maintaining a clear layout, applying consistent formatting, and focusing on business interpretation.

---

# 1. KPI Cards (Total Sales, Total Profit, Profit Margin)

### Business Question

What is the overall performance of the business?

### Why this chart?

KPI cards provide an instant summary of the most important business metrics. Executives can quickly understand the company's overall performance without analyzing detailed charts.

### Fields Used

* **Measure:** Total Sales
* **Measure:** Total Profit
* **Measure:** Profit Margin

### Design Principles Applied

* Positioned at the top of the dashboard to create a clear visual hierarchy.
* Large font size improves readability.
* Simple formatting minimizes clutter.
* Consistent formatting across all KPI cards.

### Mistake Avoided

Avoided using gauges or decorative charts, which consume more space while providing less information.

---

# 2. Monthly Sales Trend

### Business Question

How are sales changing over time?

### Chart Type

Line Chart

### Why this chart?

A line chart is the most suitable visualization for identifying trends, seasonality, and fluctuations in monthly sales.

### Fields Used

* **Columns:** Month
* **Rows:** Sales
* **Labels:** Monthly Sales
* **Filters:** Region, Category, Customer Segment

### Design Principles Applied

* Months displayed in chronological order.
* Data labels improve readability.
* Simple blue color highlights the trend.
* Clean layout without unnecessary visual elements.

### Mistake Avoided

Did not use a bar chart because it is less effective for displaying continuous trends over time.

---

# 3. Regional Sales and Profit Performance

### Business Question

Which regions generate the highest sales and profit?

### Chart Type

Horizontal Bar Chart

### Why this chart?

A horizontal bar chart allows easy comparison of sales and profit across different regions.

### Fields Used

* **Rows:** Region
* **Columns:** Measure Values (Sales and Profit)
* **Color:** Measure Names
* **Labels:** Sales and Profit values
* **Filters:** Region, Category, Customer Segment

### Design Principles Applied

* Regions are sorted based on sales.
* Different colors distinguish Sales and Profit.
* Data labels improve interpretation.

### Mistake Avoided

Avoided pie charts because comparing regional values is much easier using bars.

---

# 4. Category and Sub-Category Profitability

### Business Question

Which categories and sub-categories contribute the most profit?

### Chart Type

Horizontal Bar Chart

### Why this chart?

Bar charts clearly compare profit across multiple categories and sub-categories, making high and low performers easy to identify.

### Fields Used

* **Rows:** Sub-Category
* **Columns:** Profit
* **Color:** Category
* **Labels:** Profit
* **Filters:** Category, Region

### Design Principles Applied

* Bars sorted from highest to lowest profit.
* Consistent colors represent product categories.
* Profit values displayed on each bar.

### Mistake Avoided

Avoided stacked bars because individual sub-category comparisons become difficult.

---

# 5. Discount vs Profit Analysis

### Business Question

How does discount affect profit?

### Chart Type

Scatter Plot with Trend Line

### Why this chart?

A scatter plot is ideal for identifying relationships between two continuous variables. The trend line highlights whether higher discounts lead to lower profits.

### Fields Used

* **Columns:** Discount
* **Rows:** Profit
* **Color:** Category
* **Detail:** Order ID
* **Trend Line:** Linear Trend

### Design Principles Applied

* Discounts formatted as percentages.
* Trend lines improve interpretation.
* Different colors distinguish product categories.
* Individual orders displayed without excessive overlap.

### Mistake Avoided

Avoided aggregating the data into bars, which would hide the relationship between discount and profit.

---

# 6. Shipping Mode and Delivery Delay Impact

### Business Question

Which shipping mode experiences the longest delivery time?

### Chart Type

Horizontal Bar Chart

### Why this chart?

Bar charts provide an easy comparison of average delivery days across different shipping modes.

### Fields Used

* **Rows:** Ship Mode
* **Columns:** Average Delivery Days
* **Color:** Ship Mode
* **Labels:** Average Delivery Days
* **Filters:** Region

### Design Principles Applied

* Delivery days displayed with one decimal place.
* Simple color scheme improves readability.
* Shipping modes sorted by delivery time.

### Mistake Avoided

Avoided stacked charts because shipping modes are independent categories and should be compared directly.

---

# Dashboard Visualization Design Principles

## Correct Chart Selection

Each visualization was selected based on the business question it answers:

* Line chart for sales trends over time.
* Horizontal bar charts for comparing regions, categories, and shipping modes.
* Scatter plot for analyzing the relationship between discount and profit.
* KPI cards for summarizing overall business performance.

---

## Clear Hierarchy

The dashboard follows a logical layout:

1. KPI cards at the top provide an overall business summary.
2. Sales trend chart presents performance over time.
3. Regional and category charts compare business performance.
4. Detailed analytical charts are placed at the bottom.

This arrangement allows users to move from summary insights to detailed analysis.

---

## Minimal Clutter

* Unnecessary gridlines were removed.
* Only meaningful labels are displayed.
* White space improves readability.
* Decorative elements were avoided.

---

## Consistent Color Usage

* Consistent colors are used throughout the dashboard.
* Similar measures use the same colors wherever possible.
* Category colors remain consistent across visualizations.

---

## Proper Labels

* Every chart includes a descriptive title.
* Axes are clearly labeled.
* Data labels are shown where appropriate.
* KPI values are prominently displayed.

---

## Readable Titles

Each chart title clearly communicates the purpose of the visualization and the business question it answers.

---

## Appropriate Sorting

* Categories are sorted by Profit.
* Regions are sorted by Sales.
* Shipping modes are ordered by average delivery days.

Sorting helps users quickly identify top and bottom performers.

---

## Useful Filters

The dashboard includes interactive filters for:

* Region
* Category
* Customer Segment

These filters allow users to explore the data from different business perspectives.

---

## Avoidance of Misleading Scales

* Appropriate axis scales are maintained.
* Discount values are displayed as percentages.
* Delivery time is shown using one decimal place.
* No truncated axes were used to exaggerate differences.

---

## Focus on Business Interpretation

The dashboard focuses on answering important business questions rather than simply displaying data. It enables decision-makers to identify:

* Sales trends over time.
* Best-performing regions.
* Most profitable product categories.
* Impact of discounts on profitability.
* Shipping performance.
* Overall business performance through KPI metrics.

The dashboard supports informed decision-making through clear, interactive, and business-focused visualizations.

