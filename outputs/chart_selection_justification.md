# Chart Selection Justification

## Dashboard Design Principles

The dashboard was designed following Tableau visualization best practices. Each chart was selected based on the business question it answers, using simple layouts, consistent formatting, meaningful colors, and interactive filters to support executive decision-making.

---

## 1. Monthly Sales Trend

**Business Question**
How are sales changing throughout the year?

**Chart Type**
Line Chart

**Reason**
A line chart clearly shows monthly trends, seasonal fluctuations, and overall sales direction.

**Fields Used**
- Columns: Order Month
- Rows: Sales
- Labels: Monthly Sales
- Trend Line: Linear Trend

**Design Principles**
- Chronological ordering
- Minimal clutter
- Sales formatted in millions
- Trend line added

**Mistake Avoided**
Did not use a bar chart because trends are easier to understand with a line chart.

---

## 2. Regional Sales and Profit Performance

**Business Question**
Which region contributes the most sales and profit?

**Chart Type**
Horizontal Bar Chart (Measure Values)

**Reason**
The horizontal bar chart allows easy comparison of Sales and Profit across regions within the same view.

**Fields Used**
- Rows: Region
- Columns: Measure Values (Sales and Profit)
- Color: Measure Names
- Labels: Sales and Profit values

**Design Principles**
- Regions sorted by Sales
- Two measures shown together
- Sales and Profit clearly labeled
- Consistent blue color shades

**Mistake Avoided**
Avoided separate charts because combining Sales and Profit provides quicker comparison.

---

## 3. Category and Sub-Category Profitability

**Business Question**
Which products generate the highest profit?

**Chart Type**
Horizontal Bar Chart

**Reason**
Bar charts are effective for comparing profitability across many sub-categories.

**Fields Used**
- Sub-Category
- Profit
- Category (Color)

**Design Principles**
- Descending sort
- Profit labels
- Category colors

**Mistake Avoided**
Avoided pie charts because comparing many categories is difficult.

---

## 4. Discount vs Profit Analysis

**Business Question**
How does discount affect profit?

**Chart Type**
Scatter Plot

**Reason**
Scatter plots best display the relationship between two continuous variables.

**Fields Used**
- X-axis: Discount
- Y-axis: Profit
- Color: Category
- Size: Sales
- Trend Lines

**Design Principles**
- Percentage formatting
- Trend lines added
- Category colors

**Mistake Avoided**
Did not use line charts because discount is not a time-based variable.

---

## 5. Shipping Mode and Delivery Delay Impact

**Business Question**
Which shipping mode takes the longest to deliver?

**Chart Type**
Horizontal Bar Chart

**Reason**
Bar charts make average delivery time comparisons very easy.

**Fields Used**
- Ship Mode
- Average Delivery Days
- Labels

**Design Principles**
- Sorted by delivery days
- Days displayed on bars
- Clear colors

**Mistake Avoided**
Avoided pie charts because delivery time is numerical data.
