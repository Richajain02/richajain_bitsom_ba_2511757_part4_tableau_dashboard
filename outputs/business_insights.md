# Task 2: Calculated Fields

To support business analysis and dashboard creation, the following calculated fields were created in Tableau:

## 1. Profit Margin

**Formula:**

```tableau
IF SUM([Sales]) = 0 THEN
    0
ELSE
    SUM([Profit]) / SUM([Sales])
END
```

**Purpose:**

Calculates the percentage of profit earned from total sales. This metric helps evaluate overall profitability and compare profit performance across regions, categories, and customer segments.

---

## 2. Cost

**Formula:**

```tableau
[Sales] - [Profit]
```

**Purpose:**

Estimates the cost associated with each order by subtracting profit from sales. This field helps analyze business expenses and understand the relationship between revenue and profitability.

---

## 3. Average Order Value

**Formula:**

```tableau
SUM([Sales]) / COUNTD([Order Id])
```

**Purpose:**

Calculates the average revenue generated per order. This KPI is useful for measuring customer purchasing behavior and comparing average spending across customer segments.

---

## 4. Return Rate

**Formula:**

```tableau
SUM([Return Flag]) / COUNT([Order Id])
```

**Purpose:**

Measures the proportion of orders that were returned. This metric helps identify categories, regions, or customer segments with higher return risk.

---

## 5. Shipping Delay Bucket

**Formula:**

```tableau
IF [Delivery Days] <= 2 THEN
    "Fast (0–2 Days)"
ELSEIF [Delivery Days] <= 5 THEN
    "Normal (3–5 Days)"
ELSE
    "Delayed (6+ Days)"
END
```

**Purpose:**

Groups delivery times into meaningful categories to evaluate shipping performance and identify areas where delivery delays may affect customer satisfaction.

---

## Additional Calculated Fields

### Returned Orders

**Formula:**

```tableau
IF [Return Flag] = 1 THEN
    "Returned"
ELSE
    "Not Returned"
END
```

**Purpose:**

Converts the binary return flag into descriptive labels for easier filtering and visualization.

---

Groups discount values into categories to analyze how different discount levels influence sales and profitability.

# Task 8: Business Insights

## Insight 1 – Monthly Sales Trend

Observation:
Sales fluctuate throughout the year, with February recording the highest monthly sales.

Evidence:
Sales increased to approximately $20.34M in February before declining in April.

Business Interpretation:
Sales appear to be influenced by seasonal demand.

Recommended Action:
Investigate marketing campaigns or seasonal events that contributed to February's strong performance.

---

## Insight 2 – Regional Performance

Observation:
The South region generates the highest sales and profit.

Evidence:
South recorded approximately $64.69M in sales and $9.99M in profit.

Business Interpretation:
The South region is the company's strongest market.

Recommended Action:
Replicate successful business strategies used in the South across other regions.

---

## Insight 3 – Product Profitability

Observation:
Technology sub-categories such as Copiers, Accessories, Phones, and Machines generate the highest profits.

Evidence:
Several Technology products exceed $6M in profit.

Business Interpretation:
Technology products are the company's most profitable offerings.

Recommended Action:
Increase inventory and promotional efforts for Technology products.

---

## Insight 4 – Customer Segment

Observation:
Home Office customers contribute the highest total sales.

Evidence:
Home Office sales exceed Consumer and Corporate segments.

Business Interpretation:
Home Office customers represent an important revenue source.

Recommended Action:
Develop loyalty programs specifically targeting Home Office customers.

---

## Insight 5 – Discount Impact

Observation:
Higher discounts generally reduce profitability.

Evidence:
Trend lines in the scatter plot slope downward as discount percentage increases.

Business Interpretation:
Large discounts reduce profit margins.

Recommended Action:
Review discount policies and encourage value-based pricing.

---

## Insight 6 – Shipping Performance

Observation:
Standard Class has the longest average delivery time.

Evidence:
Average delivery time is approximately 4.7 days.

Business Interpretation:
Long delivery times may reduce customer satisfaction.

Recommended Action:
Improve logistics efficiency for Standard Class shipments.

---

## Insight 7 – Return Pattern

Observation:
Furniture records the highest number of returned orders.

Evidence:
Return Analysis shows Furniture has more returned orders than Office Supplies and Technology.

Business Interpretation:
Furniture products may have quality, packaging, or shipping issues.

Recommended Action:
Investigate return reasons and improve product quality.

---

## Insight 8 – Business Opportunity

Observation:
Technology products generate both high sales and high profit.

Evidence:
Technology dominates the profitability rankings.

Business Interpretation:
Technology presents the greatest opportunity for future growth.

Recommended Action:
Increase marketing investment and product expansion within the Technology category.

