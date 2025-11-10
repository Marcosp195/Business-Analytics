# Business Analytics for an E-commerce Startup

## 1. Project Description
This project provides a comprehensive analysis of business metrics for an e-commerce startup. The primary objective is to analyze data from marketing, user behavior, and sales to identify unprofitable marketing channels and optimize the advertising budget.

The analysis is based on three datasets: user visit logs, order logs, and marketing cost logs, covering the period from June 2017 to May 2018.

## 2. Key Business Questions Addressed
The analysis is structured to answer the following critical business questions:

* **Product:** How do people use the product? (**DAU**, **WAU**, **MAU**, session length, user retention).
* **Sales:** When do users start buying? What is the average purchase size? How much money do they generate (**LTV**)?
* **Marketing:** How much was spent on marketing? What is the cost of acquiring a customer (**CAC**)? How profitable are the marketing investments (**ROMI**)?

## 3. Analysis Methodology
The project was carried out in a Jupyter Notebook (`Analisis de negocio.ipynb`) and followed these key steps:

### a. Data Preprocessing
* Loaded three separate CSV files (`visits`, `orders`, `costs`) into Pandas DataFrames.
* Cleaned and prepared the data by standardizing column names and converting data types, especially dates to `datetime` format.
* Enriched the data by creating new columns for time-based analysis, such as `session_date`, `session_month`, and `cohort_month`.

### b. Product Analytics
* Calculated key user engagement metrics:
    * **DAU** (Daily Active Users), **WAU** (Weekly Active Users), and **MAU** (Monthly Active Users).
    * Average Session Length (**ASL**).
    * **Sticky Factor** (DAU/MAU) to measure user retention and engagement.

### c. Sales Analytics
* Performed funnel analysis to determine the conversion time from a user's first visit to their first purchase.
* Calculated the Average Order Value (**AOV**) to understand the typical purchase size.
* Conducted a Cohort Analysis to calculate the Lifetime Value (**LTV**) of customers over time. The results were visualized using a heatmap to show cumulative LTV.

### d. Marketing Analytics
* Calculated total marketing expenditure and broke it down by acquisition source.
* Determined the Customer Acquisition Cost (**CAC**) for each marketing channel by linking costs to the number of new customers acquired.
* Calculated the Return on Marketing Investment (**ROMI**) for each source using the 6-month LTV as a benchmark to evaluate channel profitability.

## 4. Key Findings & Recommendations
**Findings:** The business shows healthy fundamentals with strong user conversion (most users buy on their first day) and good retention, with customer value more than doubling in the first year. However, the analysis revealed a significant inefficiency in marketing spend: the largest portion of the budget is allocated to **Source 3**, which has the highest **CAC** and the lowest **ROMI**. In contrast, **Source 1** is the most profitable channel.

**Recommendation:** It is recommended to reallocate the marketing budget by reducing spending on the underperforming **Source 3** and increasing investment in the most profitable channels: **Source 1**, followed by **Sources 2 and 5**. This strategic shift will optimize costs and maximize the return on investment.

## 5. Technologies and Libraries Used
* **Python 3**
* **Pandas:** For data manipulation and analysis.
* **Seaborn & Matplotlib:** For generating graphs and visualizations.
