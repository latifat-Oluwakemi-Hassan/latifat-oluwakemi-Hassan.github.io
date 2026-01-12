---
layout: default
title:  E-commerce-End-to-End Data Analytics Platform
permalink: /projects/ E-commerce-End-to-End Data Analytics Platform/
---

# Customer Churn Prediction

*Problem:* The business had transaction data but lacked insight into customer churn drivers, profitable products and regions, and operational inefficiencies limiting growth.

*Solution:* Built a comprehensive end-to-end analytics platform that integrated data engineering, analysis, dashboards, and predictive modeling to generate actionable insights and enable data-driven decision-making.

## Approach

1.**Database Design & Integration:** Designed a relational database and integrated large-scale historical data for analysis.
2.**ETL & EDA:** Built an automated ETL pipeline to extract, clean, transform, and load analytics-ready tables, enabling exploratory data analysis.
3. **Business Analysis:** Analyzed customer behavior, churn patterns, regional performance, product profitability, and operational bottlenecks.
4. **Visualization:** Created interactive dashboards highlighting churn metrics, revenue trends, fulfillment efficiency, and payment failures.
5. **Modeling:** Developed a customer churn prediction model using RFM features (with recency as a key driver) and built a customer lifetime value (LTV) model to identify high-value customers.
6 **Deployment & Automation:** Deployed a web application that allows users to upload a database and instantly access dashboards and insights, with automated generation of stakeholder-ready PDF reports.

## Results

- Identified a “leaky bucket” retention pattern as a primary driver of customer churn.
- Uncovered declining sales and profit trends impacting long-term growth.
- Exposed delivery and payment inefficiencies affecting customer experience and revenue.
- Demonstrated that a small segment of high-value customers contributes the majority of future revenue.
- Enabled early churn detection and more effective customer prioritization through churn and LTV models.

## Code Highlights

```python
# Feature engineering example  
            def _normalize_missing(s):
                return s.replace(
                to_replace=["", "none", "nan", "null", "n/a", "na"],
                value=np.nan,
                regex=False
            )
