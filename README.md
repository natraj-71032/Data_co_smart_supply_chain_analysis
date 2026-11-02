# DataCo Smart Supply Chain Analytics | End-to-End Data Analyst Project

An end-to-end business intelligence project analyzing sales, profitability, customer behavior, product performance, and delivery risk for DataCo Global using **Excel, SQL, Python, and Power BI**.

> **Business focus:** Find where revenue turns into profit, identify where performance breaks down, and recommend data-driven actions to improve supply-chain efficiency and customer experience.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Business Problem](#business-problem)
- [Business Objectives](#business-objectives)
- [Tools and Technologies](#tools-and-technologies)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Dashboard Pages](#dashboard-pages)
- [Key Findings](#key-findings)
- [Business Recommendations](#business-recommendations)
- [Important Metric Definitions](#important-metric-definitions)
- [Repository Structure](#repository-structure)
- [How to Run the Project](#how-to-run-the-project)
- [Limitations and Validation Notes](#limitations-and-validation-notes)
- [Skills Demonstrated](#skills-demonstrated)

---

## Project Overview

DataCo Global operates across multiple markets, product categories, customer segments, and shipping modes. Its order-level data can be used to investigate commercial performance and supply-chain reliability.

This project uses a repeatable analytics workflow to prepare and analyze the dataset, answer business questions with SQL and Python, and communicate the results through an interactive Power BI dashboard.

The analysis is organized around two priorities:

1. **Commercial performance:** Understand which markets, customer segments, categories, and products contribute to sales and profit—and where revenue may not translate into strong profitability.
2. **Delivery performance:** Identify where late-delivery risk is concentrated across shipping modes, markets, and regions, then recommend where logistics teams should investigate first.

### Dashboard at a glance

The Power BI report contains six pages:

1. Executive Overview
2. Product Performance
3. Customer & Market Analysis
4. Delivery & Logistics Analysis
5. Insights & Recommendations
6. [Optional: add another page here if your report contains one]

Add screenshots of the report in the `images/` folder and embed them in this README so visitors can preview the work without opening Power BI.

---

## Business Problem

DataCo Global needs to understand both **profitability** and **delivery reliability** to make better decisions about product investment, inventory, markets, and logistics.

### Question 1: Where is the business generating revenue and profit—and where are sales not translating into profitability?

The analysis uses an overall profit margin of **10.78%** as a starting point for comparing categories, products, customer segments, and markets. Segment-level comparisons can help inform pricing, discount policy, product strategy, and inventory prioritization.

### Question 2: What patterns are associated with late-delivery risk?

The report indicates a late-delivery-risk rate of **54.83%**. The analysis investigates how the risk varies by shipping mode, market, and region to help operations teams prioritize further investigation into fulfillment planning, logistics processes, and service quality.

Without a structured analysis, decisions about inventory, market investment, and customer retention may rely too heavily on intuition rather than evidence.

---

## Business Objectives

- Measure overall sales, profit, profit margin, order volume, and customer count.
- Compare sales and profitability across markets, customer segments, product categories, and products.
- Identify top-performing and underperforming commercial areas.
- Examine customer purchasing patterns and repeat-customer behavior.
- Compare shipping modes and investigate delivery risk across markets and regions.
- Build an interactive Power BI report with filters for business users.
- Convert the findings into practical recommendations and questions for further investigation.

---

## Tools and Technologies

| Tool | Purpose |
|---|---|
| **Excel** | Initial data inspection, data-quality checks, and quick exploratory summaries |
| **SQL (MySQL)** | Business queries, aggregations, joins, customer and market analysis, and logistics analysis |
| **Python (Pandas, NumPy, Matplotlib/Seaborn)** | Data cleaning, exploratory data analysis (EDA), validation, and visual exploration |
| **Power BI** | Interactive dashboards, KPI cards, charts, slicers, and business storytelling |
| **GitHub** | Version control and project documentation |

*Only list libraries and techniques you actually used in the final repository.*

---

## Dataset

**Dataset:** DataCo Smart Supply Chain dataset.

The dataset contains order and order-item information, including sales, profit, product categories, customer segments, markets, countries, shipping modes, delivery status, and shipping-time fields.

Dataset details recorded for this project:

- **Rows:** 180,519 order-line records
- **Columns:** 53
- **Date coverage:** 2015 to January 2018
- **Data type:** Supply-chain, sales, customer, product, and logistics data

### Data availability

The original raw CSV is not included in this repository because it exceeds GitHub's recommended maximum file size for a regular Git repository. This repository should include the dataset source, instructions for obtaining it, and the code needed to reproduce the analysis—not a large raw-data file committed directly to Git.

**Dataset source:** Add the original dataset's public source page here. Confirm that the source and its terms permit redistribution or linking before publishing.

**To reproduce the project:**
1. Obtain the dataset from the cited source.
2. Place the CSV in the local data folder specified in the project instructions.
3. Run the cleaning and analysis steps described below.
4. Connect Power BI to the prepared data or refresh the report using the documented data model.

Do not upload customer-sensitive or otherwise restricted data.

---

## Project Workflow

### 1. Business understanding
- Defined the commercial-performance and delivery-risk questions.
- Identified the KPIs and dimensions needed to answer them.
- Mapped the intended findings to decisions that a business team could make.

### 2. Data inspection and preparation
- Checked the dataset structure, data types, missing values, duplicate records, and inconsistent categories.
- Reviewed date fields and numeric columns.
- Investigated whether order-level and order-item-level records were being counted appropriately.
- Documented cleaning and transformation decisions so the analysis can be reproduced.

### 3. Exploratory data analysis in Python
- Examined distributions and summary statistics.
- Compared sales and profit by market, category, and customer segment.
- Investigated delivery-risk patterns by shipping mode and geography.
- Used charts to identify patterns requiring deeper SQL analysis.

### 4. SQL analysis
SQL queries were organized into business-focused analysis areas, including:

- Overall business performance
- Customer and market performance
- Customer segments and repeat purchasing
- Product and category performance
- Shipping mode and delivery performance
- Late-delivery risk by market and region

### 5. Power BI reporting
- Created KPI cards for headline measures.
- Built comparative charts for markets, categories, products, customer segments, and shipping modes.
- Added slicers to support interactive exploration.
- Organized the report into pages for executives, product teams, customer/market analysis, logistics, and recommendations.

### 6. Insights and recommendations
- Summarized the strongest visible patterns.
- Linked each recommendation to an observed metric or comparison.
- Identified validation needs before treating an association as a cause.

---

## Dashboard Pages

### 1. Executive Overview
Provides a high-level view of sales, profit, orders, customers, products, market performance, order status, and monthly trends.

**Business use:** Quickly understand overall performance and identify areas that need deeper analysis.

### 2. Product Performance
Compares product categories and products by orders, sales, quantity sold, and profit.

**Business use:** Support assortment reviews and identify products or categories for further profitability and inventory analysis.

### 3. Customer & Market Analysis
Compares customer segments, markets, countries, and customer-related measures.

**Business use:** Identify where sales are concentrated and where customer or market performance deserves further investigation.

### 4. Delivery & Logistics Analysis
Examines average shipping time, late-delivery risk, delivery status, shipping modes, and geographic patterns.

**Business use:** Help logistics teams identify where to investigate service-level problems and operational bottlenecks.

### 5. Insights & Recommendations
Brings key findings together with proposed actions, including category prioritization, shipping-process improvement, market strategy, and customer retention.

**Business use:** Translate analysis into a decision-oriented summary.

### Dashboard screenshots

Save your Power BI screenshots under `images/` using the filenames below, or update the paths to match your repository.

```text
images/
├── executive-overview.png
├── product-performance.png
├── customer-market-analysis.png
├── delivery-logistics-analysis.png
└── insights-recommendations.png
```

Then embed them in the README:

```markdown
![Executive Overview](images/executive-overview.png)
![Product Performance](images/product-performance.png)
![Customer and Market Analysis](images/customer-market-analysis.png)
![Delivery and Logistics Analysis](images/delivery-logistics-analysis.png)
![Insights and Recommendations](images/insights-recommendations.png)
```

---

## Key Findings

The following are the headline findings currently displayed in the dashboard. Recalculate and validate them against the final model before publishing, particularly after applying filters or changing aggregation logic.

| Metric or finding | Dashboard result | Why it matters |
|---|---:|---|
| Total sales | 36.78M | Indicates the overall sales scale |
| Total profit | 3.97M | Provides the overall reported profit figure |
| Overall profit margin | 10.78% | Baseline for comparing profitability |
| Total orders | 65.752K | Indicates order volume |
| Total customers | 21K | Indicates customer reach |
| Late-delivery-risk rate | 54.83% | Highlights a substantial delivery-risk signal |
| Average shipping days | 3.50 | Summarizes actual shipping duration |
| Total products | 118 | Shows the breadth of the product assortment |
| Largest market by sales | Europe | Identifies the leading market in the displayed report |
| Highest-sales customer segment | Consumer | Identifies the largest segment by sales |
| Leading category by sales/profit in the displayed report | Fishing | Indicates a category for closer commercial analysis |
| Largest customer segment by profit | Consumer | Identifies the leading segment by reported profit |

### Additional patterns shown in the report

- Standard Class has the largest shipment/order volume and the highest displayed count of late deliveries.
- Consumer generates the largest displayed sales and profit contribution among customer segments.
- Europe is the largest displayed market by sales.
- Fishing leads the displayed category comparison for sales and profit.
- Repeat customers represent **56.98%** of the customer base in the current dashboard.

**Important interpretation note:** A high number of late deliveries in a shipping mode may partly reflect that mode's high order volume. Compare both the *number* of late deliveries and the *late-delivery rate* before deciding which mode performs worst. Likewise, sales leadership does not automatically mean the highest profit margin.

---

## Business Recommendations

These are proposed actions based on the patterns displayed in the report. They should be treated as hypotheses to validate—not proof of root cause.

### 1. Prioritize delivery-risk investigation
Start with shipping modes and markets that have both high shipment volume and a high late-delivery rate. Review dispatch timing, carrier performance, fulfillment capacity, and scheduled-versus-actual shipping time.

**Measure:** Late-delivery rate, late shipments, average delay, and on-time delivery rate.

### 2. Evaluate category profitability before expanding inventory
Fishing is a leading category in the displayed sales/profit charts. Review its margin, discounting, stock availability, returns (if available), and demand variability before increasing inventory.

**Measure:** Sales, profit, profit margin, quantity sold, and inventory/stockout measures if available.

### 3. Compare market growth with profitability
Europe leads the displayed sales comparison. Compare its profit margin and delivery performance with other markets before assigning additional budget or promotional spend.

**Measure:** Sales growth, profit growth, profit margin, order volume, and late-delivery rate.

### 4. Strengthen customer retention
The dashboard indicates a substantial repeat-customer share. Investigate repeat purchase frequency, customer lifetime value, order recency, and segment-level profitability to identify retention opportunities.

**Measure:** Repeat-customer rate, purchase frequency, average order value, and customer-level profit.

### 5. Review shipping-mode performance using rates, not only totals
Standard Class has the largest displayed volume. Its late-delivery count should be evaluated alongside its shipment share and late-delivery rate to distinguish a volume effect from a performance problem.

**Measure:** Shipment share, late-delivery rate, average actual shipping days, and average scheduled shipping days.

### 6. Establish a recurring KPI review
Track sales, profit margin, repeat-customer rate, average shipping time, and late-delivery rate by month and market. Investigate unusual changes rather than relying only on lifetime totals.

**Measure:** Monthly KPI trends, target variance, and exception counts.

---

## Important Metric Definitions

Use consistent definitions across SQL, Python, and Power BI. Confirm whether the dashboard is aggregating at the order-item, order, or shipment level.

| Metric | Suggested definition | Caution |
|---|---|---|
| Total sales | Sum of the sales field at the chosen grain | Confirm that records are not duplicated by joins |
| Total profit | Sum of the dataset's order-profit field | Confirm what the source field represents and whether it is repeated across order items |
| Profit margin | Total profit ÷ total sales × 100 | Do not average row-level margin percentages |
| Total orders | Count of distinct order IDs | A single order may contain multiple order-item rows |
| Total customers | Count of distinct customer IDs | Define the treatment of missing customer IDs |
| Late-delivery-risk rate | Share of records/orders with `Late_delivery_risk = 1`, according to the chosen grain | This flag may represent predicted/assigned risk, not necessarily a verified actual late-delivery outcome |
| Actual shipping days | Average of `Days for shipping (real)` | Check missing values and the grain of the records |
| Average order value | Sales ÷ distinct orders | Aggregate sales at a compatible grain |
| Repeat-customer rate | Customers with more than one distinct order ÷ customers with at least one order × 100 | Define the date window and customer population |

### Data-quality and analytical caution

The dataset contains order-item records, so **row counts, distinct orders, and distinct shipments are not interchangeable**. If order-level fields are repeated across several items, summing them directly can inflate totals. Validate the grain and aggregation logic before treating headline metrics as definitive.

Also, a `Late_delivery_risk` flag should not automatically be described as the actual late-delivery rate unless the source definition supports that interpretation. Where possible, compare it with the delivery-status field and actual versus scheduled shipping dates.

---

## Repository Structure

Adapt this example to the actual files in your GitHub repository:

```text
dataco-supply-chain-analytics/
├── README.md
├── data/
│   └── README.md                 # Dataset source and local setup instructions
├── excel/
│   └── [Excel analysis files]
├── sql/
│   ├── customer_market_analysis.sql
│   ├── logistics_delivery_analysis.sql
│   └── [other SQL analysis files]
├── python/
│   ├── [eda notebook or script]
│   └── [cleaning notebook or script]
├── powerbi/
│   └── [Power BI report file, if distributable]
└── images/
    ├── executive-overview.png
    ├── product-performance.png
    ├── customer-market-analysis.png
    ├── delivery-logistics-analysis.png
    └── insights-recommendations.png
```

Replace bracketed placeholders with the exact filenames in your repository. Remove folders or tools that are not actually included.

---

## How to Run the Project

1. **Clone or download the repository.**
2. **Obtain the dataset** from the source linked in `data/README.md` and place it in the documented local path.
3. **Inspect and prepare the data** using the Excel/Python steps included in the repository.
4. **Load the prepared data into MySQL** using the schema and import instructions you document.
5. **Run the SQL scripts** in the order described in the SQL folder's README or comments.
6. **Open the Power BI report** and update the data-source path/credentials as needed.
7. **Refresh the report** and verify the KPIs against SQL outputs.
8. **Compare the results** with the findings documented here, accounting for filters, data grain, and any transformation differences.

Add exact setup commands, database import instructions, and the Power BI file name once they are confirmed in the repository.

---

## Limitations and Validation Notes

- The dataset covers a historical period (2015 to January 2018); its findings should not be assumed to represent current supply-chain conditions.
- Observed associations do not establish causation. For example, a market with more late deliveries may also have a much higher shipment volume.
- The meaning of each delivery flag should be verified against the dataset's documentation.
- Profit, sales, orders, and shipment counts must be aggregated at compatible grains.
- The dashboard's headline figures should be revalidated after every data transformation and report filter change.
- Recommendations should be tested using operational data and agreed KPIs before implementation.

---

## Skills Demonstrated

- Business problem framing and KPI definition
- Data cleaning and exploratory data analysis
- SQL aggregations, grouping, conditional logic, and customer/market analysis
- Python-based analysis and visualization
- Power BI dashboard design and data storytelling
- Sales, profit, customer, product, and logistics analysis
- Turning findings into practical, measurable recommendations
- Documentation, reproducibility, and GitHub project presentation

---

## Project Summary

This project demonstrates how a Data Analyst can combine data preparation, SQL analysis, Python exploration, and Power BI visualization to investigate two practical business challenges: **profitable growth and delivery reliability**.

The objective is not simply to build charts. It is to define the right business questions, validate the underlying metrics, explain what the evidence shows, and recommend the next actions a business team should investigate.

---

