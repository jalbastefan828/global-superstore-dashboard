# Problem Framing

## 1. Business Strategy

### Context & Methodology
Business Strategy means understanding the company's main goals and knowing where the management wants to go. This step helps narrow down the analysis focus and prevents wasting time on irrelevant topics. It directly decides which Key Performance Indicators (KPIs) to track, who the stakeholders are, and how project success is measured. Finally, it helps prioritize data projects based on the real financial value they bring to the business.

Since this is a personal project, I simulated a real-world business environment using AI. Based on the dataset's primary operational focus, the stakeholder highlighted three high-level business challenges to guide this analysis.

### High-Level Business Questions
- We are giving too many discounts and losing money in some places. How can we fix our discount strategy to stay profitable?
- Shipping costs are too high and delivery options look messy. How can we optimize shipping modes and order priorities?
- We are seeing a lot of product returns across different customer types. Which customers or products are causing this, and why?

<br>
<br>

## 2. Product & Domain Knowledge

### Overview
Global Superstore is a fictional global e-commerce dataset that simulates a large-scale retail business. The store operates internationally (across US, APAC, EMEA, and LATAM markets), selling a wide variety of physical goods to both B2B (business-to-business) and B2C (business-to-consumer) customers.

### E-commerce Domain & Catalog
The business operates in the global online retail industry, managing order processing, international logistics, and product returns. The product catalog is divided into 3 main categories:

- _**Office Supplies:**_ High-volume, lower-cost items (paper, binders, appliances, labels).
- _**Furniture:**_ Heavy, bulky items (chairs, tables, bookcases) with higher shipping and handling costs.
- _**Technology:**_ High-value items (phones, copiers, machines) with higher price points and sensitive profit margins.

### Customer Segments
The business serves 3 main customer segments:
- _**Consumer:**_ Individual retail customers purchasing for personal use.
- _**Corporate:**_ Small and medium-sized businesses buying in larger quantities.
- _**Home Office:**_ Freelancers and remote professionals with specific home-office requirements.

### Operational Flow & Key Dynamics
- _**Order Lifecycle:**_ Order Placed -> Order Priority Assigned -> Warehouse Processing -> Selected Shipping Method -> Delivery -> (Potential) Return.
- _**Shipping Modes:**_ 4 fulfillment options (_Same Day_, _First Class_, _Second Class_, _Standard Class_).
- _**Domain Specifics:**_ Profitability in global e-commerce depends heavily on balancing shipping fees, localized discounts, and return rates.

<br>
<br>

## 3. Data Knowledge

### Overview & Definition
Data Knowledge means understanding the origin, structure, and limitations of the dataset. It ensures that variables are not treated just as random numbers or text, but as meaningful operational metrics (such as distinct data types, timestamps, and order identifiers).

### Dataset Structure & Granularity
* **Source Dataset:** Global Superstore Sales Dataset (https://www.kaggle.com/datasets/shekpaul/global-superstore).
* **Level of Granularity:** Each row in the dataset represents an **individual order line item** (a specific product purchased within an order).
* **Scope:** Contains transactional records with customer details, order locations, shipping modes, sales figures, discounts, profits, and product categories.

### Data Dictionary Reference
> **Note:** For a complete and detailed description of all fields, including data types (e.g., `Category`, `Int64`, `Float64`) and business definitions, please refer to the data dictionary spreadsheet located in the same directory

<br>
<br>

## 4. Question and Hypotheses
### Overview & Importance
Formulating key business questions and testable hypotheses is the engine of Exploratory Data Analysis (EDA). Instead of exploring the dataset blindly, this step helps break down high-level management concerns into specific, actionable analytical goals. 

By testing these hypotheses against the data, we can uncover root causes behind financial losses, validate business assumptions, and guide strategic decision-making with concrete numbers.

### A. We are giving too many discounts and losing money in some places. How can we fix our discount strategy to stay profitable?
* **Q1:** What is the overall distribution of discounts?
* **Q2:** In percentages, what are the highest applied discounts?
* **Q3:** On average, which countries and markets (regions) have the highest discounts?
* **Q4:** On average, which categories and sub-categories have the highest discounts?
* **Q5:** What do the summary statistics for discounts look like (Min, Q1, Mean, Median/Q2, Q3, Max)?
* **Q6:** If we eliminate discounts higher than 50%, how much does profit increase, and how many losing sales become profitable?
* **Q7:** Should I use a what-if analysis to change discount percentages and run test scenarios?
* **Q8:** How have discounts evolved and changed year over year?
* **Q9:** Is there any relationship between discounts and other values in the table (e.g., profit, sales, market, region, delivery time)?
* **Q10:** Are discounts affected by shipping mode and order priority?

### B. Shipping costs are too high and delivery options look messy. How can we optimize shipping modes and order priorities?
* **Q1:** What is the overall distribution of shipping costs?
* **Q2:** What do the summary statistics for shipping costs look like by category and sub-category, and which products are the most expensive to ship?
* **Q3:** How do shipping costs compare across different shipping modes and order priorities?
* **Q4:** Are there financial losses caused specifically by high shipping costs? If so, what are they?
* **Q5:** On average, which markets, regions, and countries have the highest shipping costs?
* **Q6:** How are shipping costs affected when combining destination (country, region, market) with product category and sub-category?
* **Q7:** What is the relationship between delivery time and shipping cost?
* **Q8:** What is the relationship between shipping cost and the actual sales value of the product?
* **Q9:** Is there a relationship between shipping cost and other variables in the dataset? How do factors like region, product category, product price, quantity, or shipping mode influence shipping costs?
* **Q10:** What new insights about shipping costs can we discover using What-If analysis and Pareto charts?

### C. High product return rates are affecting our revenue across different customer segments. What are the root causes and how can we reduce them?
* **Q1:** Which countries, regions, and markets have the highest number of returned items?
* **Q2:** Which customer segments or specific customers generate the most returns?
* **Q3:** How has the number of returns evolved over time (monthly and yearly trends)?
* **Q4:** Which product categories and sub-categories experience the highest return rates?
* **Q5:** What do the summary statistics of returned products look like when grouped by country, category, order priority, and shipping mode?
* **Q6:** Is there a relationship between high return rates and other variables in the dataset (e.g., shipping costs, delivery delays, discounts)?
* **Q7:** How significantly is overall profit affected when accounting for returned orders and their associated shipping costs?

<br>
<br>

## 5. Key Performance Indicators
### Overview & Importance
Key Performance Indicators (KPIs) are essential quantitative metrics used to measure business health and track progress toward core strategic goals. In this project, KPIs translate complex transactional data into clear, high-level benchmarks for executive decision-making.

Establishing well-defined metrics allows us to monitor profitability, identify operational inefficiencies in shipping, and measure the direct financial impact of product returns. These indicators serve as the foundation for the interactive dashboard and help track performance over time.

#### Core KPIs
1. **Financial & Profitability Metrics:**
   - **Total Net Profit:** Revenue minus cost of goods, shipping, and returned orders.
   - **Net Profit Margin (%):** Ratio of net profit to total sales.
   - **Average Profit per Order (AOV Profit):** Mean profit generated per single order.
   - **Average Profit per Customer:** Customer-level profitability contribution.

2. **Shipping & Logistics Metrics:**
   - **Total Shipping Cost:** Aggregate expenditure on order fulfillment.
   - **Shipping Cost Ratio (%):** Percentage of total sales spent on shipping.
   - **Average Shipping Cost per Order:** Mean transport expense per transaction.

3. **Return & Risk Metrics:**
   - **Return Rate (%):** Percentage of returned orders out of total orders.
   - **Financial Loss from Returns:** Total net profit lost due to returned items.


#### Analytical Dimensions (Breakdown Axes)
To gain deeper insights, each Core KPI above will be sliced and diced across the following dimensions in the interactive dashboard:

- **Temporal:** Year, Quarter, Month.
- **Geographical:** Market, Region, Country.
- **Product Hierarchy:** Category, Sub-Category.
- **Customer & Operations:** Customer Segment, Order Priority, Shipping Mode.

<br>
<br>

## 6. Feature Engineering & Target Engineering
Feature engineering is the process of creating new columns or transforming existing raw data (like calculating delivery time or profit margins) to uncover hidden patterns. Target engineering focuses on preparing the main outcome variable (like transforming Sales or encoding Returns) so machine learning algorithms can learn effectively. Together, they turn raw figures into high-value signals, making both descriptive analysis and predictive models significantly more accurate.

To enhance analytical capabilities, several derived features were created from the raw dataset:

- **Temporal Features:**
  - **Delivery Time:** Days elapsed between *Order Date* and *Ship Date*.
  - **Order Day Name, Order Month, Order Year:** Extracted date components for seasonality analysis.
  - **Is Weekend:** Flag identifying orders placed on Saturdays or Sundays.

- **Financial & Cost Metrics:**
  - **Original Price:** Estimated price before applying discounts (Sales / (1 - Discount)).
  - **Discount Value:** Absolute monetary discount granted (Original Price - Sales).
  - **Cost:** Total transaction cost (Sales - Profit).
  - **Product Cost:** Base product cost excluding logistics (Cost - Shipping Cost).

- **Business Ratios & Percentages:**
  - **Profit Margin:** Profitability relative to sales (Profit / Sales).
  - **Shipping Ratio:** Proportion of sales consumed by shipping fees (Shipping Cost / Sales).
  - **Cost Ratio:** Proportion of sales spent on total costs (Cost / Sales).

<br>
<br>

## 7. Model Selection
Model selection involves choosing, testing, and comparing different machine learning algorithms (such as Linear Regression, Decision Trees, or Logistic Regression) to find the best fit for our data. By selecting the right model, we can move beyond historical analysis and accurately predict future business outcomes, such as identifying high-risk returns or forecasting shipping costs.

<br>
<br>

## 8. Communication of Results
Communication of results is the final step where complex data insights, statistical findings, and model outputs are translated into clear stories for stakeholders. Through interactive dashboards, structured summaries, and visual charts, this step ensures that analytical findings directly answer the key business questions and drive actionable strategic decisions.