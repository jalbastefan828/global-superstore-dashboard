# Exploratory Data Analysis (EDA) Summary

## Discount Analysis

### 1. Market Analysis

* **EMEA:** Discounts apply to *32.62%* of products. The **p75 is at 60%**, and the **maximum is 70%**, generating a **profit erosion of 83.77%**.
* **Africa:** *77% of orders are at full price* (**p75 = 0.0%**), but the remaining *23%* have discounts up to **70%**. The average discount is **16%**, and profit erosion reaches **61.27%**.
* **US & APAC:** More than half of the orders have discounts (**APAC: 58.62%**, **US: 51.99%**). These are the only markets with a **median discount greater than 0**.
* **LATAM vs. EU:** LATAM applies discounts to **41.60%** of orders (**p75 = 40%**), with an erosion of **63.75%**. EU applies discounts to **38.47%** of orders (**p75 = 10%**), with an erosion of **56.31%**.
* **Canada:** **0% discounts** and low order volume (*control group with pure margin*).

### 2. Country Analysis

#### Top Countries with Net Losses (CASH LOSSES)

* **Turkey (EMEA):** **1,378 orders** (*100% discounted*). Fixed discount: **60%**. Net loss: **-$98,447.23**. Total discounts given: **$162,761.94**. Profit erosion: **253.07%**.
* **Nigeria (Africa):** **905 orders** (*100% discounted*). Fixed discount: **70%**. Net loss: **-$80,750.72**. Total discounts given: **$126,817.48**. Profit erosion: **275.29%**.
* **Netherlands (EU):** **407 orders** (*100% discounted*). Average discount: **48%** (**median 50%**). Net loss: **-$38,991.19**. Total discounts given: **$70,962.91**.
* **Honduras (LATAM):** **681 orders** (*100% discounted*). Average discount: **41%** (**minimum 40%**). Net loss: **-$27,247.99**. Total discounts given: **$61,958.53**.
* **Pakistan (APAC):** **242 orders** (*100% discounted*). Average discount: **45%** (**maximum 80%**). Net loss: **-$21,805.67**. Total discounts given: **$49,899.20**. Profit erosion: **177.62%**.
* **Argentina (LATAM):** **369 orders** (*100% discounted*). Average discount: **43%** (**minimum 40%**, **maximum 70%**). Net loss: **-$18,085.47**.
* **Panama (LATAM):** **378 orders** (*100% discounted*). Average discount: **41%** (**minimum 40%**). Net loss: **-$17,545.28**.
* **Sweden (EU):** **195 orders** (*100% discounted*). Average discount: **51%** (**minimum 50%**). Net loss: **-$17,023.56**. Profit erosion: **206.55%**.
* **Philippines (APAC):** **651 orders** (*100% discounted*). Average discount: **35%** (between *15% and 55%*). Net loss: **-$14,682.76**. Total discounts given: **$79,659.55**.
* **Venezuela (LATAM):** **181 orders** (*100% discounted*). Average discount: **41%** (**minimum 40%**). Net loss: **-$11,029.88**. Profit erosion: **199.49%**.

#### Other Regional Country Insights

* **Turkmenistan, Kazakhstan, Tajikistan, Yemen, UAE, Lithuania:** The top 9 countries globally by profit erosion (**Turkmenistan: 331.43%**, **Kazakhstan: 294.72%**, **Tajikistan: up to 331.43%**) have a **fixed discount of 70%** applied to all orders.
* **Uganda:** **37 orders**, fixed discount **70%**, net loss **-$2,426.08**, profit erosion: **278.59%**.
* **Indonesia:** **1,315 orders** (*100% discounted*), positive net profit: **+$14,900**. Minimum discount: **7%**, median: **27%**, discount losses: **$113,000**.
* **Australia:** **94.46% of orders have a discount**. Average discount: **14%**, median: **10%**. Net profit: **+$99,504**. Profit erosion: **60.76%**.
* **USA (Detailed):** **5,196 discounted products** (**51.99%**), maximum discount: **80%**. Actual profit: **$286,397.03**. Total discounts: **$566,734.19**. Profit erosion: **66.43%** (out of a potential *$853,131.19*).
* **Dominican Republic:** **712 orders** (*100% discounted*). Average discount: **24%** (**minimum 20%**). Net loss: **-$5,597.44**. Profit erosion: **113.58%**.
* **Portugal:** *100% discounted orders* with a **fixed discount of 50%**. Profit erosion: **235.94%**.

### 3. Category and Sub-Category Analysis

#### By Category

* **Furniture:** **54.41% discounted products**. Actual profit: **$264,704.59** (out of a potential *$1.16 million*). Profit erosion: **77.25%**.
* **Technology:** **47.94% discounted products**. Maximum discount: **70%**. Net profit: **$623,635.62**. Profit erosion: **54.41%**.
* **Office Supplies:** **38.98% discounted products** (*over 18,000 orders without discount*). Maximum discount: **80%**. Profit erosion: **56.87%**.

#### By Sub-Category

* **Tables:** Net profit: **-$61,118.64** (*the only sub-category in the negative*). Discounted orders: **75.49%** (**p25 = 20%**). Average discount: **29%**. Profit erosion: **124.83%**.
* **Discount Penetration Rate (% discounted orders):** **Tables (75.49%)**, **Chairs (61.40%)**, **Copiers (59.87%)**, **Bookcases (53.00%)**, **Phones (50.09%)**, **Machines (49.26%)**.
* **Profit Erosion on Other Sub-Categories:** **Machines (78.12%)**, **Binders (69.14%)**.
* **Resistance to Discounting:** **Paper** (*32.37% erosion*) and **Labels** (*39.99% erosion*), both having *over 63% of orders sold without a discount*.

### 4. Top Volume Customer Analysis

* The top 5 customers by volume of discounted orders (**Greg Matthias, Carlos Soltero, Harry Greene, Joy Smith, Tracy Blumstein**) have *over 53% of products bought at a discount*.
* These customers receive **maximum discounts between 60% and 80%**, leading to a **profit erosion of over 100%** and generating *direct net financial losses*.

### 5. Correlation Analysis (Exact Numbers)

* **Discount vs. Quantity:** Values between **-0.07 and 0.03** (*almost zero correlation across all dimensions*).
* **Discount vs. Shipping Cost:** Values between **-0.26 and 0.00** (*very low correlation*).
* **Discount vs. Profit Margin:** Values between **-0.77 and -0.94** (*extremely strong negative correlation*).

#### Discount vs. Absolute Profit Correlation by Market

* **LATAM:** **-0.42**
* **Africa:** **-0.39**
* **EMEA:** **-0.38**
* **APAC:** **-0.36**
* **US:** **-0.22**
* **Canada:** **NaN** (*0% discount*)

#### Discount vs. Profit Margin Correlation by Market

* **Africa:** **-0.94**
* **EMEA:** **-0.91**
* **APAC:** **-0.77**

#### Sub-Category Correlations

* **Tables:** **-0.68** with absolute profit and **-0.26** with shipping cost.
* **Binders:** **-0.17** with absolute profit and **-0.89** with profit margin.
* **Other High Correlations with Profit:** **Fasteners (-0.61)**, **Bookcases (-0.56)**, **Envelopes (-0.54)**.

#### Operational Groupings (order_priority, order_day_name, ship_mode)

* Discount vs. Profit Margin Correlation: fixed between **-0.83 and -0.85**.
* Discount vs. Quantity Correlation: between **-0.03 and 0.03**.
* Discount vs. Shipping Cost Correlation: between **-0.07 and -0.09**.