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

