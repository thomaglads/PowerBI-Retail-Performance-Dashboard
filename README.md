# PowerBI-Retail-Performance-Dashboard
Retail performance analysis using Power BI, showcasing insights into sales drivers, customer segmentation, and profitability from simulated data.
# Retail Performance Dashboard: Sales, Profitability & Trends

## Objective
This project involved creating an interactive dashboard using Power BI to analyze a simulated retail dataset. The primary goal was to gain insights into sales performance, customer behavior, and profitability drivers, such as product category performance, purchase mediums, loyalty program impact, and customer experience.

## Live Dashboard / Screenshot
Below is a screenshot of the final dashboard.
            ![image](https://github.com/user-attachments/assets/53ba04df-507d-4dc1-8013-d795e50d1c35)
![Screenshot 2025-06-01 172935](https://github.com/user-attachments/assets/b72d505a-b04c-4e45-9937-085ea9edab5a)


**Key Visualizations Include:**
* **KPIs:** Overall Number of Transactions, Average Customer Experience, and Total Purchases After Discount.
* **Decomposition Tree:** To interactively explore the drivers of "Total Purchases After Discount" across dimensions like Product Category, Purchase Medium, and Loyalty Program status.
* **Sales Trends:** A time-series line chart showing "Total Purchases After Discount by Year, Quarter, Month and Day."
* **Purchase Medium Breakdown:** A pie chart illustrating the proportion of "Total Purchases After Discount" by online vs. in-store channels.

## Data Source
The data used for this project is the **"Sales Simulation"** dataset, sourced from Kaggle:
[Sales Simulation Dataset on Kaggle](https://www.kaggle.com/datasets/noeyislearning/sales-simulation)

This synthetic dataset is designed to simulate customer purchase behavior and includes detailed information on:
* Customer Demographics (age, sex, country - primarily Philippines in this dataset)
* Purchase Details (product category, purchase medium, transaction dates)
* Loyalty Program (participation status, tier, points redeemed, discounts)
* Discounts and Payments (total discounts, payment methods, final purchase amounts)
* Customer Experience (customer experience rating for each transaction)
* Logistics (shipping methods, costs, delivery days)

The dataset contains over 380,000 transaction records. For this analysis, key date columns (`joined_date`, `payment_date`, `purchased_date`, `released_date`, `estimated_delivery_date`, `received_date`) were transformed to proper date types, and anomalies in fields like `total_delivery_days` were addressed during the data preparation phase in Power Query.

## Tools Used
* **Power BI Desktop:** For data import, data transformation (Power Query), data modeling, DAX measure creation, and interactive dashboard development.
* **DAX (Data Analysis Expressions):** Used to create key calculated measures such as:
    * `Total Purchases After Discount`
    * `Number of Transactions`
    * `Average Customer Experience`
    * (and potentially others like `Total Gross Profit` as seen in earlier chart versions if you kept it)
* **Python with Pandas via Jupyter Notebook:** For initial data exploration and overview.

## Key Features & Functionality Developed
* **Data Cleaning and Transformation:** Processed date columns into correct formats and handled data anomalies  negative delivery days using Power Query.
* **Calculated Measures:** Developed DAX measures to accurately summarize key business metrics.
* **Interactive Exploration:** Utilized a Decomposition Tree to allow for dynamic drill-down into the main sales metric (`Total Purchases After Discount`) by various attributes like product category, purchase medium, and loyalty status.
* **Trend Analysis:** Visualized sales performance over time to identify patterns.
* **Categorical & Segment Analysis:** Broke down sales by purchase medium and provided KPIs for customer experience and transaction volume.
* **User-Friendly Design:** Implemented a clear, dark-themed layout for easy readability and professional presentation.

## Skills Demonstrated
* Data Analysis & Visualization (Power BI)
* Data Cleaning and Preparation (Power Query)
* Data Modeling (Implicit in Power BI for single table, or explicit if you created a date table)
* DAX for creating calculated measures
* Dashboard Design & Storytelling
* Analysis of Customer Behavior (purchase medium, customer experience, loyalty)
* Retail & Sales Analytics

---
