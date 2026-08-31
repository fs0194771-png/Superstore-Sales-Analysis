# Superstore Sales Analysis

## Project Overview

This project analyzes Superstore sales transaction data from 2019 to 2022 to evaluate overall business performance and identify the main factors affecting profitability.

The main objective is to understand why the business generates high sales but still operates at a net loss, and to identify the key areas that can be improved to increase profitability.

---

## Business Problem

The company generates significant sales revenue, but its overall profitability is negative.

This analysis aims to answer the following business questions:

- How is the business performing overall?
- Which categories and sub-categories are profitable or loss-making?
- How does discounting affect profitability?
- Which products and areas contribute most to losses?
- How does profitability change over time?
- Are profitability problems concentrated in specific regions or cities?
- Which customer segments are more or less profitable?
- Does shipping time have a significant impact on profitability?

---

## Dataset

The dataset contains **9,994 sales transaction records** covering the period from **2019 to 2022**.

It includes information about:

- Customers
- Products
- Categories and sub-categories
- Customer segments
- Geographic locations
- Sales
- Quantity
- Discounts
- Profit
- Shipping information

### Dataset Overview

- **Records:** 9,994
- **Original Columns:** 21
- **Categories:** 3
- **Sub-categories:** 17
- **Customer Segments:** 3
- **Regions:** 4
- **Time Period:** 2019–2022

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Workflow

The analysis follows a structured data analysis workflow:

1. Business Understanding
2. Data Understanding
3. Data Cleaning
4. Data Wrangling
5. Exploratory Data Analysis (EDA)
6. Data Visualization
7. Business Insights
8. Recommendations
9. Conclusion

---

## Data Understanding

The dataset was inspected to understand its:

- Structure and dimensions
- Column names
- Data types
- Unique values
- Statistical characteristics
- Missing values
- Duplicate records

The dataset contains **9,994 records** covering sales transactions from **2019 to 2022**.

---

## Data Cleaning

The following data cleaning and validation steps were performed:

- Checked for missing values
- Checked for duplicate rows
- Standardized column names
- Converted date columns to datetime format
- Validated data types
- Validated important numeric ranges
- Checked the relationship between order dates and shipping dates

No missing values or duplicate rows were identified.

---

## Data Wrangling

Additional analytical columns were created from the existing data to support the analysis, including:

- Year
- Month
- Month Name
- Day Name
- Shipping Days
- Profit Margin

These columns were used to perform time-based, profitability, and business performance analysis.

---

# Exploratory Data Analysis (EDA)

The EDA focused on identifying the main drivers of profitability across different business dimensions.

## Overall Business Performance

The business generated:

- **Total Sales:** $5.76M
- **Total Gains:** $348.50K
- **Total Losses:** -$438.82K
- **Net Profit:** -$90.32K
- **Overall Profit Margin:** -1.57%
- **Total Quantity:** 35,018
- **Total Customers:** 793
- **Average Discount:** 28.74%

The analysis shows that the business generates strong sales revenue but fails to convert those sales into overall profit.

---

# Key Business Insights

## 1. Category Performance

Technology generated the highest profit at approximately **$64.55K**, while Office Supplies achieved the highest profit margin at **4.73%**.

Furniture was the main source of losses, generating approximately **$2.36M in sales** while recording a loss of approximately **$199.12K**, resulting in a profit margin of **-8.45%**.

This demonstrates that high sales volume does not necessarily translate into high profitability.

---

## 2. Sub-category Performance

All four Furniture sub-categories were loss-making:

- **Tables:** -$50.65K
- **Chairs:** -$51.13K
- **Furnishings:** -$49.25K
- **Bookcases:** -$48.09K

The losses are therefore not isolated to a single product group but represent a broader profitability problem within the Furniture category.

---

## 3. Discount and Profitability

Profitability decreases significantly as discounts increase.

At **0% discount**, the business generated approximately **$250.18K profit** with a **14.70% profit margin**.

Profit became negative starting at approximately **30% discount**, and reached a loss of approximately **$106.10K** at an **80% discount**.

The correlation between discount and profit was:

**-0.46**

The correlation between discount and profit margin was:

**-0.92**

This indicates a strong negative relationship between discounting and profitability.

---

## 4. Discount Impact Across Categories

The impact of discounts differs between categories.

Furniture becomes loss-making at a relatively low discount level, with its profit margin becoming negative at approximately **15% discount**.

Technology also becomes loss-making at higher discount levels, while Office Supplies remains profitable for longer.

This suggests that discount policies should be customized by category rather than applying the same discount strategy across the entire business.

---

## 5. Yearly Performance

Sales remained relatively stable across the four years, ranging from approximately **$1.37M to $1.49M**.

However, profitability varied considerably.

**2020 was the worst-performing year**, with:

- **Sales:** $1.49M
- **Profit:** -$38.82K
- **Profit Margin:** -2.61%

Since average discounts were relatively similar across years, the decline in 2020 cannot be explained by average discount alone.

---

## 6. Year × Category Performance

Furniture remained loss-making across every year.

Its worst performance occurred in 2020:

- **Profit:** -$55.63K
- **Profit Margin:** -9.19%

This suggests that the Furniture profitability problem is structural rather than being limited to a single year.

---

## 7. Regional Performance

Furniture generated losses across all four regions.

The largest Furniture losses occurred in:

- **East:** -$63.32K
- **West:** -$60.88K
- **Central:** -$47.02K
- **South:** -$27.90K

This confirms that the Furniture profitability problem is not limited to a single region.

---

## 8. City Performance

Several cities recorded significant overall losses.

City-level analysis indicates that profitability problems are concentrated in certain locations and should be evaluated together with product, category, and discount performance.

---

## 9. Customer Profitability

Some customers generated relatively high sales while still producing significant losses.

The highest loss-making customers recorded losses ranging from approximately **$1.82K to $3.03K**.

This shows that high-revenue customers are not necessarily profitable customers.

---

## 10. Customer Segment Performance

All three customer segments were unprofitable:

- **Consumer:** -$38.30K
- **Corporate:** -$25.17K
- **Home Office:** -$26.86K

Home Office recorded the worst profit margin at approximately **-2.66%**.

Therefore, profitability problems exist across all customer segments.

---

## 11. Shipping Performance

Shipping duration did not show a clear relationship with profitability.

All shipping-duration groups remained loss-making, but there was no consistent pattern indicating that longer shipping times directly caused higher losses.

Therefore, shipping time does not appear to be a major driver of the company's profitability problem.

---

## 12. Monthly Performance

The business remained loss-making across all months.

The strongest monthly results were observed around:

- September
- July
- March

The weakest months included:

- August
- June
- January
- May

However, there was no strong seasonal pattern capable of explaining the overall profitability problem.

---

# Data Visualization

The following visualizations highlight the most important findings from the analysis.

## 1. Profit by Category

![Profit by Category](./Profit%20by%20Category.png)

This visualization highlights the profitability difference between the three major categories and shows the significant loss generated by Furniture.

---

## 2. Sales by Category

![Sales by Category](./Sales%20by%20Category.png)

This visualization compares sales across categories and demonstrates that high sales do not necessarily result in high profit.

---

## 3. Discount vs Profit Margin

![Discount vs Profit Margin](./Discount%20vs%20Profit%20Margin.png)

This visualization shows the strong negative relationship between discount levels and profit margin.

---

## 4. Profit by Year

![Profit by Year](./Profit%20by%20Year.png)

This visualization shows how profitability changed from 2019 to 2022 and highlights the significant decline in 2020.

---

## 5. Profit by Sub-Category

![Profit by Sub-Category](./Profit%20by%20Sub-Category.png)

This visualization highlights the profitability of individual sub-categories and shows the losses generated by the Furniture sub-categories.

---

## 6. Monthly Profit

![Monthly Profit](./Monthly%20Profit.png)

This visualization shows the monthly profitability pattern and helps identify stronger and weaker periods throughout the year.

---

# Recommendations

## 1. Reassess the Discount Strategy

Reduce excessive discounting, particularly discounts of **30% or more**, where profitability becomes negative in the overall analysis.

Discount decisions should consider:

- Product profitability
- Category
- Customer value
- Demand
- Existing profit margin

---

## 2. Review the Furniture Category

Furniture should be the highest priority for profitability improvement.

The company should investigate:

- Product costs
- Pricing
- Supplier costs
- Discount levels
- Product-level margins
- Consistently unprofitable products

---

## 3. Apply Category-Specific Discount Policies

A single discount strategy should not be applied across all categories.

Furniture requires stricter discount controls because it becomes unprofitable at relatively low discount levels.

---

## 4. Review Loss-Making Furniture Sub-categories

Since all four Furniture sub-categories are loss-making, management should review the pricing and cost structure of the entire Furniture category.

---

## 5. Investigate High-Loss Products

Products with high sales but strongly negative profit margins should be reviewed individually.

Possible actions include:

- Increasing prices
- Reducing discounts
- Negotiating supplier costs
- Discontinuing consistently unprofitable products

---

## 6. Investigate the 2020 Profitability Decline

Since sales remained relatively stable while profitability declined significantly in 2020, additional operational, pricing, product-mix, or discount-related factors should be investigated.

---

## 7. Focus on Profitable Categories

Technology and Office Supplies should be maintained and potentially expanded.

However, future growth should be evaluated based on **profitability rather than sales volume alone**.

---

## 8. Monitor Customer Profitability

Customers should be evaluated based on profit generated, not revenue alone.

High-revenue customers generating repeated losses should be reviewed for:

- Excessive discounts
- Product mix
- Order size
- Pricing conditions

---

## 9. Investigate High-Loss Locations

Cities and regions with significant losses should be investigated to determine whether the issue is related to:

- Product mix
- Discounting
- Pricing
- Customer behavior
- Operating costs

---

## 10. Do Not Prioritize Shipping Changes as the Main Solution

Since shipping duration did not show a clear relationship with profitability, reducing shipping time should not be considered the primary solution.

The analysis indicates that **pricing, discounting, and product profitability** are more important areas to address.

---

# Conclusion

The analysis shows that the company's main challenge is not generating sales, but converting sales into profit.

Despite generating approximately **$5.76M in sales**, the business recorded a **net loss of $90.32K** and an overall profit margin of **-1.57%**.

Furniture is the primary source of losses, while Technology and Office Supplies remain profitable.

The analysis also revealed a strong negative relationship between discounting and profitability, with profit margins declining sharply as discounts increase.

The profitability problem exists across different years, regions, cities, and customer segments, while shipping duration does not appear to be a major driver.

Therefore, the main opportunities for improvement are:

- Controlling excessive discounts
- Restructuring the Furniture category
- Reviewing loss-making products
- Monitoring customer and location profitability
- Focusing growth on profitable products and categories rather than sales volume alone

---

# Project Structure

```text
Superstore-Sales-Analysis/
│
├── Superstore_Sales.csv
├── Superstore_Sales_Analysis.ipynb
│
├── Profit by Category.png
├── Sales by Category.png
├── Discount vs Profit Margin.png
├── Profit by Year.png
├── Profit by Sub-Category.png
├── Monthly Profit.png
│
└── README.md
