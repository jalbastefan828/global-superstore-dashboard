# Exploratory Data Analysis (EDA) Summary

# Discount Analysis

## 1. Overview
* The average discount across the entire dataset is 14%.
* 43.71% of products have at least one discount applied, with 25% receiving discounts greater than 20%.
* Overall profit erosion is reaching 62.44%.
* While total profit shows a weak correlation with discounts, there is an extremely strong negative correlation between profit margin and discounts (-0.85).
* There is no relationship between discounts and order quantity or shipping costs.
* The actual overall profit margin is 11.43%, compared to a potential profit margin of 25.58% without discounts.


## 2. Market Analysis

* **EMEA:** Discounts apply to 32.62% of products. The p75 is at 60%, and the maximum is 70%, generating a profit erosion of 83.77%.
* **Africa:** 77% of orders are at full price (p75 = 0.0%), but the remaining 23% have discounts up to 70%. The average discount is 16%, and profit erosion reaches 61.27%.
* **US & APAC:** More than half of the orders have discounts (APAC: 58.62%, US: 51.99%). These are the only markets with a median discount greater than 0.
* **LATAM vs. EU:** LATAM applies discounts to 41.60% of orders (p75 = 40%), with an erosion of 63.75%. EU applies discounts to 38.47% of orders (p75 = 10%), with an erosion of 56.31%.
* **Canada:** 0% discounts and low order volume.

## 3. Country Analysis

### Top Countries with Net Losses

* **Turkey (EMEA):** 1,378 orders (100% discounted). Fixed discount: 60%. Net loss: -$98,447.23. Total discounts given: $162,761.94. Profit erosion: 253.07%.
* **Nigeria (Africa):** 905 orders (100% discounted). Fixed discount: 70%. Net loss: -$80,750.72. Total discounts given: $126,817.48. Profit erosion: 275.29%.
* **Netherlands (EU):** 407 orders (100% discounted). Average discount: 48% (median 50%). Net loss: -$38,991.19. Total discounts given: $70,962.91.
* **Honduras (LATAM):** 681 orders (100% discounted). Average discount: 41% (minimum 40%). Net loss: -$27,247.99. Total discounts given: $61,958.53.
* **Pakistan (APAC):** 242 orders (100% discounted). Average discount: 45% (maximum 80%). Net loss: -$21,805.67. Total discounts given: $49,899.20. Profit erosion: 177.62%.
* **Argentina (LATAM):** 369 orders (100% discounted). Average discount: 43% (minimum 40%, maximum 70%). Net loss: -$18,085.47.
* **Panama (LATAM):** 378 orders (100% discounted). Average discount: 41% (minimum 40%). Net loss: -$17,545.28.
* **Sweden (EU):** 195 orders (100% discounted). Average discount: 51% (minimum 50%). Net loss: -$17,023.56. Profit erosion: 206.55%.
* **Philippines (APAC):** 651 orders (100% discounted). Average discount: 35% (between 15% and 55%). Net loss: -$14,682.76. Total discounts given: $79,659.55.
* **Venezuela (LATAM):** 181 orders (100% discounted). Average discount: 41% (minimum 40%). Net loss: -$11,029.88. Profit erosion: 199.49%.

### Other Regional Country Insights

* **Turkmenistan, Kazakhstan, Tajikistan, Yemen, UAE, Lithuania:** The top 9 countries globally by profit erosion (Turkmenistan: 331.43%, Kazakhstan: 294.72%, Tajikistan: up to 331.43%) have a fixed discount of 70% applied to all orders.
* **Uganda:** 37 orders, fixed discount 70%, net loss -$2,426.08, profit erosion: 278.59%.
* **Indonesia:** 1,315 orders (100% discounted), positive net profit: +$14,900. Minimum discount: 7%, median: 27%, discount losses: $113,000.
* **Australia:** 94.46% of orders have a discount. Average discount: 14%, median: 10%. Net profit: +$99,504. Profit erosion: 60.76%.
* **USA (Detailed):** 5,196 discounted products (51.99%), maximum discount: 80%. Actual profit: $286,397.03. Total discounts: $566,734.19. Profit erosion: 66.43% (out of a potential *$853,131.19*).
* **Dominican Republic:** 712 orders (100% discounted). Average discount: 24% (minimum 20%). Net loss: -$5,597.44. Profit erosion: 113.58%.
* **Portugal:** 100% discounted orders with a fixed discount of 50%. Profit erosion: 235.94%.

## 4. Category and Sub-Category Analysis

### By Category

* **Furniture:** 54.41% discounted products. Actual profit: $264,704.59 (out of a potential $1.16 million). Profit erosion: 77.25%.
* **Technology:** 47.94% discounted products. Maximum discount: 70%. Net profit: $623,635.62. Profit erosion: 54.41%.
* **Office Supplies:** 38.98% discounted products (over 18,000 orders without discount). Maximum discount: 80%. Profit erosion: 56.87%.

### By Sub-Category

* **Tables:** Net profit: -$61,118.64 (the only sub-category in the negative). Discounted orders: 75.49% (p25 = 20%). Average discount: 29%. Profit erosion: 124.83%.
* **Discounted orders (%):** Tables (75.49%), Chairs (61.40%), Copiers (59.87%), Bookcases (53.00%), Phones (50.09%), Machines (49.26%).
* **Profit Erosion (%):** Machines (78.12%), Binders (69.14%).
* **Resistance to discounting:** Paper (32.37% erosion) and Labels (39.99% erosion), both having over 63% of orders sold without a discount.

## 5. Top Volume Customer Analysis

* The top 5 customers by volume of discounted orders (Greg Matthias, Carlos Soltero, Harry Greene, Joy Smith, Tracy Blumstein) have over 53% of products bought at a discount.
* These customers receive maximum discounts between 60% and 80%, leading to a profit erosion of over 100% and generating direct net financial losses.

## 6. Correlation Analysis

* **Discount vs Quantity:** Values between -0.07 and 0.03 (almost zero correlation across all dimensions).
* **Discount vs Shipping Cost:** Values between -0.26 and 0.00 (very low correlation).
* **Discount vs Profit Margin:** Values between -0.77 and -0.94 (extremely strong negative correlation).

### Discount vs Profit by Market

* **LATAM:** -0.42
* **Africa:** -0.39
* **EMEA:** -0.38
* **APAC:** -0.36
* **US:** -0.22
* **Canada:** NaN (0% discount)

### Discount vs Profit Margin by Market

* **Africa:** -0.94
* **EMEA:** -0.91
* **APAC:** -0.77

### Sub-Category Correlations

* **Tables:** -0.68 with profit and -0.26 with shipping cost.
* **Binders:** -0.17 with profit and -0.89 with profit margin.
* **Other high correlations with profit:** Fasteners (-0.61), Bookcases (-0.56), Envelopes (-0.54).

### Operational Groupings (order_priority, order_day_name, ship_mode)

* **Discount vs Profit Margin:** fixed between -0.83 and -0.85.
* **Discount vs Quantity:** between -0.03 and 0.03.
* **Discount vs Shipping Cost:** between -0.07 and -0.09.

## 7. Time-Series Analysis

* Even though profit increases year over year, 2013 has the lowest profit erosion rate and the fewest discounted orders (42.84%). On the other hand, 2014, which has the highest total profit and is the last year, ranks second in terms of profit erosion and number of discounted products. The same pattern applies to the profit margin: 2014 has an actual profit margin of 11.54% (with a potential of 25.53%), while 2013 achieves an actual profit margin of 11.89% (with a potential of 25.61%).
* The worst year is the first one, 2011, which had the highest share of discounted products (44.49%) and the largest profit erosion (65.54%). It recorded an actual profit margin of only 10.90%, despite a very high potential of 26.21% (in fact, 2011 had the highest potential profit margin, meaning it lost the most money because of discounts).
* Overall, we can see higher numbers for total profit and profit margin each year, as well as lower profit erosion. The only exception is between 2013 and 2014: even though 2014 made the highest total profit, 2013 was better at controlling and managing discounts.

<br><br><br>

# Shipping cost Analysis

## 1. Overview

- 75% of orders have a shipping cost of $24.14 or less. The remaining 25% of orders cost between $24.14 and $933.57.
- The average shipping cost is $26.17 (with a median of $7.69 and a total cost of $1,283,490.75).
- The average shipping ratio is 0.1092. This means that, on average, the shipping cost is about 11% of the final price (for example, a $100 product costs around $11 to ship).
- 50% of orders have a shipping ratio below 9.02%, while the other 50% are above 9.02%. Additionally, 25% of orders have a shipping ratio higher than 13.64%.

## 2. Correlation & ANOVA Analysis

- **Shipping Cost vs. Quantity:** The correlation is 0.27, which means the number of items ordered has only a small impact on the shipping cost.
- **Shipping Cost vs. Sales:** The correlation is 0.77, showing that higher sales values usually come with higher shipping costs.
- **Shipping Cost vs. Profit:** The correlation is 0.35, indicating a weak positive relationship between shipping costs and profit.
- **Shipping Cost vs. Order Priority & Ship Mode:** Both have a p-value of 0.0 (with high F-statistics of 683.76 and 375.95). This shows a strong relationship, meaning order priority and shipping method heavily influence the shipping cost.
- **Shipping Cost vs. Country:** The p-value is 0.0, which confirms that shipping costs vary significantly depending on the destination country.
- **Shipping Cost vs. Sub-Category:** The p-value is 0.0 (F-statistic: 636.41), proving that certain product types are much more expensive to ship than others.

## 3. Order Priority Analysis

- On average, orders marked as Critical have a shipping ratio of 25% and an average shipping cost of $59.26 (more than three times higher than Medium priority).
- There is an unexpected pattern between Low and Medium priorities. Medium priority has an average shipping cost of $18.34 (8% shipping ratio), while Low priority is more expensive at $26.56 (12% shipping ratio). However, Medium and High priorities generate the highest total shipping costs ($516,293.28 and $483,552.75) due to higher order volumes.
- All four priority categories reach very similar maximum shipping costs, ranging between $867.69 and $933.57.


## 4. Ship Mode Analysis

- The distribution of shipping costs follows a logical order based on delivery speed. Same Day is the most expensive with an average cost of $42.25, followed by First Class at $40.93, Second Class at $30.33, and Standard Class at $19.78.
- Standard Class generates the highest total shipping cost ($582,988.00) because it is the most frequently used shipping method.
- There is a very small difference between Same Day and First Class, as both share the exact same average shipping ratio of 18% (and a global ratio of 17%). Even more surprisingly, the median cost for First Class ($12.58) is slightly higher than for Same Day ($12.19), meaning 50% of First Class orders cost more than $12.58, compared to $12.19 for Same Day.

## 5. Market Analysis

- All seven markets have the exact same average shipping ratio of 11% (and a median of 9%), showing a balanced pricing structure where shipping costs scale proportionally with order value across all regions.
- APAC has the highest average shipping cost at $34.93 per order, as well as the highest total shipping cost ($358,116.66), followed by the EU with an average of $30.52.
- Surprisingly, the US ranks third highest with an average shipping cost of $23.83 (and holds the highest single maximum shipping cost at $933.57), even though Global Superstore is a US-based company.
- EMEA has the lowest average shipping cost at $17.53 per order, while Canada has the lowest total shipping cost ($7,405.63) due to its very low order volume.

## 6. Country Analysis

- **Highest Average Shipping Cost:** The country with the highest average shipping cost is Taiwan ($167.36), followed by Chad ($148.97), Lesotho ($135.65), Montenegro ($93.94), and Slovenia ($61.22).
- **Top 20 Countries by Market:** Looking at the top 20 countries with the highest average shipping costs, 7 are from APAC, 7 from Africa, 5 from EMEA, and 1 from LATAM.
- **Highest Average Shipping Ratio:** Taiwan also has the highest average shipping ratio at 20% (meaning shipping represents 20% of the sales value), followed by Lebanon (17%), Central African Republic (16%), and Djibouti (15%).
- **Highest P75 Shipping Costs:** The countries with the highest P75 values are Lesotho (25% of orders cost over $284.63 to ship), Chad (25% of orders cost over $222.52), Taiwan, and Montenegro.
- **Highest Total Shipping Costs:** The countries generating the highest total shipping costs due to high order volumes are the United States ($238,173.80), Australia ($96,488.61), France ($88,502.45), China ($65,606.79), Germany ($60,686.80), and India ($59,638.01).

## 7. Category and Sub-Category Analysis

- **Shipping Ratio:** All categories and sub-categories have the exact same average shipping ratio of 11%, showing that shipping costs remain proportional to product prices across all product types.
- **Category Average Costs:** Technology has the highest average shipping cost at $49.92, followed closely by Furniture at $44.32, while Office Supplies is the cheapest category to ship at $12.80. However, due to high order volumes, Office Supplies still generates a large total shipping cost ($383,569.72), close to Furniture ($417,026.56).
- **Most Expensive Sub-Categories:** Based on average shipping cost, the most expensive sub-categories are Tables ($93.17), Copiers ($71.52), Bookcases ($63.98), Appliances ($60.27), and Phones ($54.98). Notably, 25% of Tables orders cost over $110.33 to ship, which strongly contributes to its negative net profit when combined with heavy discounts.
- **Highest Total Shipping Cost by Sub-Category:** Phones ($177,912.20), Chairs ($155,636.05), and Copiers ($149,695.47) generate the highest total shipping expenses, while Labels ($3.09 average) and Fasteners ($3.70 average) are the cheapest to ship.


## 8. Order Year Analysis

- Shipping costs remained remarkably consistent over the years. The average shipping cost stayed stable between $25.95 and $26.83, and the average shipping ratio stayed flat at 11% across all four years (2011 to 2014).


## 9. Outliers Analysis

- **High financial impact from few orders:** Although outliers represent only 8% to 10% of total orders across all sub-categories, they account for an enormous share of total shipping expenses, ranging from 33% to 60%.
- **Binders sub-category:** Binders has the highest outlier impact, where just 581 outlier orders generate 60% ($27,933.64) of the sub-category's total shipping cost.
- **Outlier Thresholds (Upper Bound):** The shipping cost threshold to be classified as an outlier varies greatly by product type, from just $7.81 for Labels to $235.67 for Tables and $188.17 for Copiers, reflecting differences in physical size and weight.


<br><br><br>

# Returned products Analysis

## 1. Overview