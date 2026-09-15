# Exploratory Data Analysis (EDA) Summary

### Order priority distribution

* **Medium:** 57.39% (29,433 orders)
* **High:** 30.22% (15,501 orders)
* **Critical:** 7.67% (3,932 orders)
* **Low:** 4.73% (2,424 orders)

> **Key Takeaway:** The vast majority of orders fall under **Medium** and **High** priority, representing **87.61%** of total volume. In contrast, the two extreme priority levels (**Critical** and **Low**) make up only a small fraction of overall operations.

---

### Order day name distribution

* **Monday:** 17.89% (9,177 orders)
* **Tuesday:** 18.15% (9,307 orders)
* **Wednesday:** 17.58% (9,017 orders)
* **Thursday:** 17.30% (8,871 orders)
* **Friday:** 18.23% (9,348 orders)
* **Saturday:** 8.93% (4,580 orders)
* **Sunday:** 1.93% (990 orders)

> **Key Insight:** Orders are evenly distributed during weekdays, peaking on **Friday** (18.23%). Order volume drops drastically on weekends, hitting a low on **Sunday** (1.93%). 
<br>89.14% of total order volume is generated during weekdays (Monday–Friday).

---

### Ship mode distribution

* **Standard Class:** 60.00% (30,775 orders)
* **Second Class:** 20.10% (10,309 orders)
* **First Class:** 14.63% (7,505 orders)
* **Same Day:** 5.27% (2,701 orders)

> **Key Insight:** **Standard Class** is the dominant shipping method (60.00%), whereas **Same Day** delivery accounts for only 5.27%.

---

### Customer segment distribution

* **Consumer (B2C):** 51.70% (26,518 orders)
* **Corporate (B2B):** 30.08% (15,429 orders)
* **Home Office (B2B / Small Business):** 18.22% (9,343 orders)

> **Key Takeaway:** Individual consumers (**B2C**) account for slightly more than half of overall demand (**51.70%**), while commercial accounts (**B2B**, combining Corporate and Home Office) represent the remaining **48.30%** of total order volume.

---

### Country Distribution (Top 25)

* **United States:** 19.49% (9,994 orders)
* **Australia:** 5.53% (2,837 orders)
* **France:** 5.51% (2,827 orders)
* **Mexico:** 5.16% (2,644 orders)
* **Germany:** 4.03% (2,065 orders)
* **China:** 3.67% (1,880 orders)
* **United Kingdom:** 3.18% (1,633 orders)
* **Brazil:** 3.12% (1,599 orders)
* **India:** 3.03% (1,555 orders)
* **Indonesia:** 2.71% (1,390 orders)
* **Turkey:** 2.69% (1,378 orders)
* **Italy:** 2.16% (1,108 orders)
* **Nigeria:** 1.76% (905 orders)
* **Spain:** 1.67% (859 orders)
* **Dominican Republic:** 1.45% (742 orders)
* **El Salvador:** 1.43% (736 orders)
* **Cuba:** 1.41% (724 orders)
* **Honduras:** 1.39% (713 orders)
* **Philippines:** 1.33% (681 orders)
* **New Zealand:** 1.22% (628 orders)
* **Nicaragua:** 1.20% (614 orders)
* **Iran:** 1.18% (607 orders)
* **Guatemala:** 1.02% (521 orders)
* **Egypt:** 0.95% (487 orders)
* **South Africa:** 0.90% (461 orders)

> **Key Takeaway:** Order distribution is heavily concentrated in the **United States**, which single-handedly accounts for nearly **19.49%** of total global demand. The remaining top markets (Australia, France, Mexico) follow with around 5% each, while the rest of the top 25 countries represent smaller individual market shares (under 4% each).
<br>The top 25 countries generate 73.18% of total global orders.

---

### Regional Distribution

* **APAC:** 21.45% (11,002 orders)
* **LATAM:** 20.07% (10,294 orders)
* **EU:** 19.50% (10,000 orders)
* **US:** 19.49% (9,994 orders)
* **EMEA:** 9.81% (5,029 orders)
* **Africa:** 8.94% (4,587 orders)
* **Canada:** 0.75% (384 orders)

> **Key Takeaway:** Order volume is remarkably balanced across four major core markets (**APAC**, **LATAM**, **EU**, and **US**), each generating roughly **19%–21%** of total demand. Secondary markets (**EMEA** and **Africa**) together account for under **19%**, while **Canada** remains a niche market at **0.75%**.

---

### Product Category Distribution

* **Office Supplies:** 60.97% (31,273 orders)
* **Technology:** 19.77% (10,141 orders)
* **Furniture:** 19.26% (9,876 orders)

> **Key Takeaway:** **Office Supplies** dominates overall order volume, accounting for **60.97%** of total demand. High-value categories (**Technology** and **Furniture**) split the remaining volume almost evenly at roughly **19.5%** each.

---

### Product Sub-Category Distribution

* **Binders:** 11.99% (6,152 orders)
* **Storage:** 9.86% (5,059 orders)
* **Art:** 9.52% (4,883 orders)
* **Paper:** 6.90% (3,538 orders)
* **Chairs:** 6.70% (3,434 orders)
* **Phones:** 6.55% (3,357 orders)
* **Furnishings:** 6.18% (3,170 orders)
* **Accessories:** 6.00% (3,075 orders)
* **Labels:** 5.08% (2,606 orders)
* **Envelopes:** 4.75% (2,435 orders)
* **Supplies:** 4.73% (2,425 orders)
* **Fasteners:** 4.72% (2,420 orders)
* **Bookcases:** 4.70% (2,411 orders)
* **Copiers:** 4.33% (2,223 orders)
* **Appliances:** 3.42% (1,755 orders)
* **Machines:** 2.90% (1,486 orders)
* **Tables:** 1.68% (861 orders)

> **Key Takeaway:** High-frequency, low-cost consumables (**Binders**, **Storage**, and **Art**) drive the highest volume, together accounting for **31.37%** of total orders. Conversely, high-ticket items like **Tables** and **Machines** account for the lowest order volume (under 3% each).

---

### Returned Status Distribution

* **False (Kept):** 94.05% (48,240 orders)
* **True (Returned):** 5.95% (3,050 orders)

> **Key Takeaway:** The overall product return rate stands at **5.95%** (3,050 orders). While seemingly low, targeted post-EDA root-cause analysis is required to determine if returns are heavily concentrated within specific product sub-categories, high-ticket items, or regional fulfillment networks.

---

### Top 5 Products by Total Revenue (Sales)

* **Apple Smart Phone, Full Size:** $86,935.78
* **Cisco Smart Phone, Full Size:** $76,441.53
* **Motorola Smart Phone, Full Size:** $73,156.30
* **Nokia Smart Phone, Full Size:** $71,904.55
* **Canon imageCLASS 2200 Advanced Copier:** $61,599.82

### Top 5 Loss-Making Products

* **Cubify CubeX 3D Printer Double Head Print:** -$8,879.97
* **Lexmark MX611dhe Monochrome Laser Printer:** -$4,589.97
* **Motorola Smart Phone, Cordless:** -$4,447.04
* **Cubify CubeX 3D Printer Triple Head Print:** -$3,839.99
* **Bevis Round Table, Adjustable Height:** -$3,649.89

> **Key Takeaway:** High-end **Technology** items (full-size smartphones and enterprise copiers) dominate gross revenue generation. However, high-ticket hardware—specifically **3D printers**, **commercial laser printers**, and **office furniture**—drives the heaviest net losses, likely inflated by aggressive regional discounting or high shipping overhead.

---

### Return Rates & Volume by Category

* **Furniture:** 6.46% return rate (638 returned items)
* **Technology:** 6.15% return rate (624 returned items)
* **Office Supplies:** 5.72% return rate (1,788 returned items)

### Return Rates by Shipping Mode

* **First Class:** 6.56% return rate
* **Same Day:** 6.41% return rate
* **Second Class:** 6.15% return rate
* **Standard Class:** 5.69% return rate

### Total Returns by Customer Segment

* **Consumer (B2C):** 1,582 returned orders
* **Corporate (B2B):** 971 returned orders
* **Home Office (B2B / Small Business):** 497 returned orders

> **Key Takeaway:** While **Office Supplies** drives the highest raw return volume (**1,788 items**) due to its high sales frequency, **Furniture** exhibits the highest relative return rate at **6.46%**. Across fulfillment methods, expedited options (**First Class** and **Same Day**) suffer higher return rates (~6.4%–6.6%) compared to **Standard Class** (5.69%), indicating potential service-level or damage risks associated with express shipments.

---

### Total Profit Breakdown

#### By Category
* **Technology:** $663,778.75
* **Office Supplies:** $518,473.84
* **Furniture:** $285,204.72

#### By Market
* **APAC:** $436,000.06
* **EU:** $372,829.75
* **US:** $286,397.03
* **LATAM:** $221,643.48
* **Africa:** $88,871.63
* **EMEA:** $43,897.97
* **Canada:** $17,817.39

#### By Customer Segment
* **Consumer (B2C):** $749,239.81
* **Corporate (B2B):** $441,208.31
* **Home Office (B2B / Small Business):** $277,009.19

#### By Order Priority
* **Medium:** $864,203.75
* **High:** $420,373.50
* **Critical:** $124,224.16
* **Low:** $58,655.85

#### By Sub-Category (Top 10 Profitable)
* **Copiers:** $258,567.55
* **Phones:** $216,717.00
* **Bookcases:** $161,924.42
* **Appliances:** $141,680.59
* **Chairs:** $140,396.27
* **Accessories:** $129,626.30
* **Storage:** $108,461.49
* **Binders:** $72,449.84
* **Paper:** $59,207.68
* **Machines:** $58,867.88

> **Key Takeaway:** Profit distribution across sub-categories highlights a clear discrepancy between order volume and net earnings. High-value tech items (**Copiers** and **Phones**) drive the highest profitability, whereas volume-heavy consumables like **Binders** (which ranked #1 in total orders) yield significantly lower bottom-line returns. High-ticket price points generally yield stronger margins than low-cost consumables.
<br> Total profitability totalizes **$1,467,457.31**. **Technology** generates the largest share of bottom-line profit (~45.2%), while **Furniture** severely lags behind due to low margins and high logistics costs. Regionally, **APAC** and **EU** lead profitability, outperforming the **US** despite similar order volumes. Across customer types, individual **Consumers** generate over half of overall profits ($749k), and **Medium priority** fulfillment accounts for the vast majority of net income ($864k).

---

### Geographic Profitability Highlights

#### Top 10 Most Profitable Countries
* **United States:** $286,397.03
* **China:** $150,683.08
* **India:** $129,071.84
* **United Kingdom:** $111,900.15
* **France:** $109,029.00
* **Germany:** $107,322.82
* **Australia:** $103,907.43
* **Mexico:** $102,818.09
* **Spain:** $54,390.12
* **El Salvador:** $42,023.24

#### Bottom 10 Least Profitable Countries
* **Turkey:** -$98,447.23
* **Nigeria:** -$80,750.72
* **Netherlands:** -$41,070.07
* **Honduras:** -$29,482.37
* **Pakistan:** -$22,446.65
* **Argentina:** -$18,693.80
* **Panama:** -$17,723.45
* **Sweden:** -$17,519.37
* **Philippines:** -$16,128.23
* **South Korea:** -$12,792.83

> **Key Takeaway:** The **United States**, **China**, and **India** lead global net profits, with the US alone generating over **$286k**. However, severe loss pools exist in key regional markets—most notably **Turkey** (-$98.4k) and **Nigeria** (-$80.7k)—where high transaction volumes are undercut by heavy discounting and operational overhead. Addressing these negative-margin regions is critical for bottom-line optimization.

---

### Feature Correlations Matrix

* **Cost vs. Product Cost:** +0.995  
  *(Base product cost directly dictates the overall cost structure.)*
* **Profit vs. Shipping Cost:** +0.354  
  *(High-value and high-margin items carry higher shipping fees.)*
* **Profit vs. Discount:** -0.316  
  *(Aggressive discounting significantly erodes net profit margins.)*
* **Delivery Time vs. Shipping Cost:** -0.143  
  *(Faster/expedited delivery times drive up operational shipping costs.)*
* **Profit vs. Quantity:** +0.104  
  *(Selling larger quantities does not automatically translate to higher profit.)*
* **Sales vs. Discount:** -0.087  
  *(Price cuts fail to effectively stimulate meaningful top-line sales growth.)*

> **Key Takeaway:** Discounting is currently counterproductive: it shows a negative correlation with both **Profit** (-0.316) and **Sales** (-0.087), proving that price cuts fail to drive volume while actively destroying margins. Conversely, shipping costs scale positively with profit (+0.354), reflecting high-value transactions rather than operational inefficiency.

---

### Average Shipping Cost by Sub-Category

* **Tables:** $92.75
* **Copiers:** $71.75
* **Bookcases:** $64.49
* **Appliances:** $61.71
* **Phones:** $55.08
* **Machines:** $53.25
* **Chairs:** $47.82
* **Accessories:** $27.16
* **Storage:** $23.83
* **Furnishings:** $12.85
* **Supplies:** $10.23
* **Art:** $8.46
* **Binders:** $7.83
* **Envelopes:** $7.62
* **Paper:** $7.54
* **Fasteners:** $3.74
* **Labels:** $3.09

> **Key Takeaway:** Heavy and bulky items—specifically **Tables** ($92.75) and **Bookcases** ($64.49)—along with high-value equipment like **Copiers** ($71.75), incur the highest average shipping costs per unit. Conversely, lightweight consumable sub-categories (**Fasteners**, **Labels**, **Paper**) maintain minimal freight overhead, staying well under $8.00 per order.

---

### Key Business Metrics Summary

**Dataset Scale**
- Total Observations & Attributes: 51,290 rows × 39 columns
- Timeframe Span: 1,430 unique days
- Global Scope: 25,035 orders across 147 countries
- Unique products: 10,292
- Total quantity sold: 178,312

**Profitability Ratio**
- Profitable Orders vs. Loss-Making Orders: 74.24% Profit / 25.76% Loss
- Overall Profit Margin: 12.00%

**Customer Metrics**
- Total Unique Customers: 1,590
- Avg. Orders / Products per Customer: 15.75 orders / 112.15 items
- Avg. Revenue / Profit per Customer: $7,951.26 Revenue / $922.93 Profit

**Order Metrics**
- Avg. Revenue / Profit per Order: $504.99 Revenue / $58.62 Profit
- Avg. Items per Order: 7.12 units (2.05 unique products)

**Operational Performance**
- Global Return Rate: 5.95%

> **Key Takeaway:** Financial performance is severely impacted by operational and strategic inefficiencies: over **25.76% of orders operate at a loss**, primarily driven by counterproductive discounting (which erodes margins without lifting volume) and high logistics costs on bulky products. Net profitability is heavily anchored by tech categories (Copiers, Phones) and core markets like the US, but is continuously drained by severe loss-making international regions (Turkey, Nigeria) and high freight overhead. Returns remain stable at ~5.95%, uninfluenced by delivery speed.

---

### Numerical Features Summary

| Metric | count | mean | std | min | 25% | 50% | 75% | max |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **delivery_time** | 51,290 | 3.97 | 1.73 | 0.00 | 3.00 | 4.00 | 5.00 | 7.00 |
| **quantity** | 51,290 | 3.48 | 2.28 | 1.00 | 2.00 | 3.00 | 5.00 | 14.00 |
| **original_price** | 51,290 | 292.58 | 600.62 | 0.99 | 38.46 | 100.92 | 296.34 | 45,276.96 |
| **discount** | 51,290 | 0.14 | 0.21 | 0.00 | 0.00 | 0.00 | 0.20 | 0.85 |
| **discount_value** | 51,290 | 46.09 | 209.26 | 0.00 | 0.00 | 0.00 | 25.51 | 22,638.48 |
| **sales** | 51,290 | 246.49 | 487.57 | 0.44 | 30.76 | 85.05 | 251.05 | 22,638.48 |
| **profit** | 51,290 | 28.61 | 174.34 | -6,599.98 | 0.00 | 9.24 | 36.81 | 8,399.98 |
| **profit_margin** | 51,290 | 0.05 | 0.47 | -4.73 | 0.00 | 0.17 | 0.33 | 0.50 |
| **cost** | 51,290 | 217.88 | 430.90 | 0.55 | 26.88 | 73.64 | 222.96 | 24,449.56 |
| **shipping_cost** | 51,290 | 26.38 | 57.30 | 0.00 | 2.61 | 7.79 | 24.45 | 933.57 |
| **product_cost** | 51,290 | 191.50 | 391.31 | 0.36 | 22.86 | 63.50 | 193.79 | 24,425.27 |
| **shipping_ratio** | 51,290 | 0.11 | 0.07 | 0.00 | 0.06 | 0.09 | 0.14 | 0.59 |
| **cost_ratio** | 51,290 | 0.95 | 0.47 | 0.50 | 0.67 | 0.83 | 1.00 | 5.73 |

> **Key Takeaway:** The data shows huge differences between normal sales and extreme cases. For example, half of all orders have sales under **$85.05**, but the highest sale reaches **$22,638.48**. While an average order brings a small profit of **$28.61**, some orders lose a lot of money—down to **-$6,599.98**. These big losses happen mostly because of high product costs and very big discounts, which reach a maximum of **85%**. Shipping costs also show extreme jumps: while **75%** of all orders have shipping costs under **$24.45**, the highest shipping cost jumps suddenly to over **$933.00**.




<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>






# Analiza Executivă a Discounturilor și Profitabilității

## 1. Analiza pe Piețe Generale (Markets)

* **EMEA:** Reduceri pe *32,62%* din produse. Procentul **p75 este la 60%**, iar **maximul la 70%**, generând o **erodare a profitului de 83,77%**.
* **Africa:** *77% din comenzi sunt la preț întreg* (**p75 = 0,0%**), dar restul de *23%* au reduceri de până la **70%**. Media discountului este de **16%**, iar erodarea profitului ajunge la **61,27%**.
* **US & APAC:** Peste jumătate dintre comenzi au reducere (**APAC: 58,62%**, **US: 51,99%**). Sunt singurele piețe cu **mediana discountului mai mare de 0**.
* **LATAM vs. EU:** LATAM aplică discounturi pe **41,60%** din comenzi (**p75 = 40%**), cu o erodare de **63,75%**. EU aplică discounturi pe **38,47%** din comenzi (**p75 = 10%**), cu o erodare de **56,31%**.
* **Canada:** **0% discounturi** și volum redus de comenzi (*grup de control cu marjă pură*).

## 2. Analiza pe Țări

### Top Țări cu Pierderi Net (CASH LOSSES)

* **Turcia (EMEA):** **1.378 comenzi** (*100% reduse*). Discount fix: **60%**. Pierdere netă: **-$98.447,23**. Discounturi acordate: **$162.761,94**. Erodare profit: **253,07%**.
* **Nigeria (Africa):** **905 comenzi** (*100% reduse*). Discount fix: **70%**. Pierdere netă: **-$80.750,72**. Discounturi acordate: **$126.817,48**. Erodare profit: **275,29%**.
* **Olanda (EU):** **407 comenzi** (*100% reduse*). Discount mediu: **48%** (**mediana 50%**). Pierdere netă: **-$38.991,19**. Discounturi acordate: **$70.962,91**.
* **Honduras (LATAM):** **681 comenzi** (*100% reduse*). Discount mediu: **41%** (**minim 40%**). Pierdere netă: **-$27.247,99**. Discounturi acordate: **$61.958,53**.
* **Pakistan (APAC):** **242 comenzi** (*100% reduse*). Discount mediu: **45%** (**maxim 80%**). Pierdere netă: **-$21.805,67**. Discounturi acordate: **$49.899,20**. Erodare profit: **177,62%**.
* **Argentina (LATAM):** **369 comenzi** (*100% reduse*). Discount mediu: **43%** (**minim 40%**, **maxim 70%**). Pierdere netă: **-$18.085,47**.
* **Panama (LATAM):** **378 comenzi** (*100% reduse*). Discount mediu: **41%** (**minim 40%**). Pierdere netă: **-$17.545,28**.
* **Suedia (EU):** **195 comenzi** (*100% reduse*). Discount mediu: **51%** (**minim 50%**). Pierdere netă: **-$17.023,56**. Erodare profit: **206,55%**.
* **Filipine (APAC):** **651 comenzi** (*100% reduse*). Discount mediu: **35%** (între *15% și 55%*). Pierdere netă: **-$14.682,76**. Discounturi acordate: **$79.659,55**.
* **Venezuela (LATAM):** **181 comenzi** (*100% reduse*). Discount mediu: **41%** (**minim 40%**). Pierdere netă: **-$11.029,88**. Erodare profit: **199,49%**.

### Alte Specificități Regionale pe Țări

* **Turkmenistan, Kazahstan, Tadjikistan, Yemen, UAE, Lituania:** Primele 9 țări la nivel global ca erodare a profitului (**Turkmenistan: 331,43%**, **Kazahstan: 294,72%**, **Tadjikistan: până la 331,43%**) au un **discount fix de 70%** aplicat pe toate comenzile.
* **Uganda:** **37 comenzi**, discount fix **70%**, pierdere netă **-$2.426,08**, erodare profit: **278,59%**.
* **Indonezia:** **1.315 comenzi** (*100% reduse*), profit net pozitiv: **+$14.900**. Discount minim: **7%**, mediana: **27%**, pierderi din discount: **$113.000**.
* **Australia:** **94,46% din comenzi au reducere**. Discount mediu: **14%**, mediana: **10%**. Profit net: **+$99.504**. Erodare profit: **60,76%**.
* **SUA (detaliat):** **5.196 produse reduse** (**51,99%**), discount maxim: **80%**. Profit real: **$286.397,03**. Discounturi totale: **$566.734,19**. Erodare profit: **66,43%** (din potențialul de *$853.131,19*).
* **Republica Dominicană:** **712 comenzi** (*100% reduse*). Discount mediu: **24%** (**minim 20%**). Pierdere netă: **-$5.597,44**. Erodare profit: **113,58%**.
* **Portugalia:** *100% comenzi reduse* cu **discount fix de 50%**. Erodare profit: **235,94%**.

## 3. Analiza pe Categorii și Sub-Categorii

### Pe Categorii Mari

* **Furniture:** **54,41% produse reduse**. Profit real: **264.704,59 $** (din potențialul de *1,16 milioane $*). Erodare profit: **77,25%**.
* **Technology:** **47,94% produse reduse**. Discount maxim: **70%**. Profit net: **623.635,62 $**. Erodare profit: **54,41%**.
* **Office Supplies:** **38,98% produse reduse** (*peste 18.000 comenzi fără discount*). Discount maxim: **80%**. Erodare profit: **56,87%**.

### Pe Sub-Categorii

* **Tables:** Profit net: **-$61.118,64** (*singura sub-categorie pe minus*). Comenzi cu discount: **75,49%** (**p25 = 20%**). Discount mediu: **29%**. Erodare profit: **124,83%**.
* **Rata de penetrare a discountului (% comenzi reduse):** **Tables (75,49%)**, **Chairs (61,40%)**, **Copiers (59,87%)**, **Bookcases (53,00%)**, **Phones (50,09%)**, **Machines (49,26%)**.
* **Erodare profit pe alte sub-categorii:** **Machines (78,12%)**, **Binders (69,14%)**.
* **Rezistență la discount:** **Paper** (*erodare 32,37%*) și **Labels** (*erodare 39,99%*), ambele având *peste 63% din comenzi vândute fără reducere*.

## 4. Analiza pe Clienți Top Volum

* Primii 5 clienți după volumul de comenzi cu discount (**Greg Matthias, Carlos Soltero, Harry Greene, Joy Smith, Tracy Blumstein**) au *peste 53% din produse cumpărate la reducere*.
* Acești clienți primesc **discounturi maxime între 60% și 80%**, având o **erodare a profitului de peste 100%** și generând *pierderi financiare nete directe*.

## 5. Analiza de Corelație (Cifre Exacte)

* **Discount vs. Cantitate (quantity):** Valori între **-0,07 și 0,03** (*corelație aproape zero pe toate dimensiunile*).
* **Discount vs. Cost Transport (shipping_cost):** Valori între **-0,26 și 0,00** (*corelație foarte mică*).
* **Discount vs. Marjă Profit (profit_margin):** Valori între **-0,77 și -0,94** (*corelație negativă extrem de puternică*).

### Corelație Discount vs. Profit Absolut pe Piețe (Markets)

* **LATAM:** **-0,42**
* **Africa:** **-0,39**
* **EMEA:** **-0,38**
* **APAC:** **-0,36**
* **US:** **-0,22**
* **Canada:** **NaN** (*discount 0%*)

### Corelație Discount vs. Marjă Profit pe Piețe (Markets)

* **Africa:** **-0,94**
* **EMEA:** **-0,91**
* **APAC:** **-0,77**

### Corelații pe Sub-Categorii

* **Tables:** **-0,68** cu profitul absolut și **-0,26** cu costul de transport.
* **Binders:** **-0,17** cu profitul absolut și **-0,89** cu marja de profit.
* **Alte corelații mari cu profitul:** **Fasteners (-0,61)**, **Bookcases (-0,56)**, **Envelopes (-0,54)**.

### Grupări Operaționale (Zile, Ship Mode, Customer Segment, Order Priority)

* Corelația discount vs. marjă profit: fixă între **-0,83 și -0,85**.
* Corelația discount vs. cantitate: între **-0,03 și 0,03**.
* Corelația discount vs. cost transport: între **-0,07 și -0,09**.

