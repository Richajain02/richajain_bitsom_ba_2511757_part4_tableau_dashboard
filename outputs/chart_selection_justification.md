# Chart Selection Justification

## 1. Sales Trend View

**Business Question:**  
How are sales changing over time?

**Chart Type:**  
Line Chart

**Reason for Selection:**  
A line chart is the most appropriate visualization for displaying sales trends over time. It clearly shows increases, decreases, and seasonal patterns, enabling leadership to monitor business growth.

**Fields Used:**
- X-Axis: Order Date (Month)
- Y-Axis: Sales
- Color: Single color for consistency
- Tooltip: Sales, Profit, Profit Margin

**Design Principles Applied:**
- Chronological order maintained.
- Minimal clutter with clear axis labels.
- Sales values formatted in millions.
- High and low sales points highlighted.

**Mistake Avoided:**
Avoided using bar charts, which are less effective for identifying time-based trends.

---

## 2. Regional Performance View

**Business Question:**  
Which regions perform best in terms of sales and profit?

**Chart Type:**  
Horizontal Bar Chart using Measure Names and Measure Values

**Reason for Selection:**  
A horizontal bar chart using Measure Names and Measure Values enables leadership to compare multiple performance metrics (Sales and Profit) for each region within a single visualization. This approach provides a side-by-side comparison, making it easy to identify regions with high sales but lower profitability and regions that perform well on both metrics.

**Fields Used:**
- Rows: Region
- Columns: Measure Values
- Measure Names: Filtered to Sales and Profit
- Color: Measure Names
- Tooltip: Sales, Profit, Profit Margin

**Design Principles Applied:**
- Regions are sorted for easy comparison.
- Consistent color coding differentiates Sales and Profit.
- Clear labels and values formatted in millions improve readability.
- A single chart reduces dashboard clutter by combining two related metrics.

**Mistake Avoided:**
Avoided creating two separate charts for Sales and Profit, which would consume more dashboard space and make comparison less efficient.

---

## 3. Category Profitability View

**Business Question:**  
Which categories and sub-categories generate the highest and lowest profits?

**Chart Type:**  
Horizontal Bar Chart

**Reason for Selection:**  
A bar chart effectively compares profitability across multiple sub-categories while allowing easy identification of profitable and loss-making products.

**Fields Used:**
- Y-Axis: Sub-Category
- X-Axis: Profit
- Color: Category
- Tooltip: Sales, Profit, Profit Margin

**Design Principles Applied:**
- Bars sorted from highest to lowest profit.
- Clear labels and consistent colors.
- Minimal visual clutter.

**Mistake Avoided:**
Avoided treemaps because precise comparisons are more difficult.

---

## 4. Customer Segment Performance

**Business Question:**  
Which customer segment contributes the most sales?

**Chart Type:**  
Horizontal Bar Chart

**Reason for Selection:**  
A bar chart enables quick comparison of sales across customer segments and clearly identifies the highest contributing segment.

**Fields Used:**
- Y-Axis: Customer Segment
- X-Axis: Sales
- Color: Customer Segment
- Tooltip: Sales, Profit, Profit Margin

**Design Principles Applied:**
- Sorted by sales.
- Consistent formatting.
- Easy-to-read labels.

**Mistake Avoided:**
Avoided pie charts because small differences between segments are easier to compare using bars.

---

## 5. Shipping Performance View

**Business Question:**  
Which shipping mode has the longest average delivery time?

**Chart Type:**  
Horizontal Bar Chart

**Reason for Selection:**  
A horizontal bar chart provides a clear comparison of average delivery days across different shipping modes.

**Fields Used:**
- Y-Axis: Ship Mode
- X-Axis: Average Delivery Days
- Color: Ship Mode
- Tooltip: Average Delivery Days, Sales, Profit

**Design Principles Applied:**
- Sorted by delivery time.
- Labels formatted to one decimal place.
- Consistent colors.

**Mistake Avoided:**
Avoided stacked bars, which could misrepresent average delivery times.

---

## 6. Discount vs Profit Analysis

**Business Question:**  
How does discount affect profit?

**Chart Type:**  
Scatter Plot

**Reason for Selection:**  
A scatter plot is the best choice for showing the relationship between two continuous variables. It reveals patterns, clusters, and loss-making orders at higher discount levels.

**Fields Used:**
- X-Axis: Discount
- Y-Axis: Profit
- Color: Category
- Detail: Order ID
- Trend Line: Enabled

**Design Principles Applied:**
- Trend line added to highlight the overall relationship.
- Percentage formatting applied to discount values.
- Minimal clutter with consistent colors.

**Mistake Avoided:**
Avoided line and bar charts because they do not effectively display relationships between continuous variables.

---

## 7. Return Analysis View

**Business Question:**  
Which categories and customer segments have the highest number of returns?

**Chart Type:**  
Stacked Horizontal Bar Chart

**Reason for Selection:**  
A stacked bar chart allows comparison of total returned orders while showing the contribution of each customer segment.

**Fields Used:**
- Y-Axis: Category
- X-Axis: Returned Orders
- Color: Customer Segment
- Tooltip: Returned Orders

**Design Principles Applied:**
- Clear labels.
- Consistent color usage.
- Easy comparison across categories.

**Mistake Avoided:**
Avoided pie charts because they make it difficult to compare return counts across multiple categories.

---

## Dashboard Design Principles

The dashboard follows key visualization best practices by using appropriate chart types, consistent color schemes, descriptive titles, readable labels, business-friendly formatting, interactive filters, and dashboard actions. The layout minimizes clutter while allowing leadership to quickly identify sales trends, regional performance, profitability, customer behavior, shipping efficiency, discount impact, and return patterns.
