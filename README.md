Customer Shopping Behavior Analysis
Overview

This project analyzes customer shopping behavior using a complete data analytics workflow. The goal is to extract business insights from purchase data by performing data exploration, cleaning, SQL analysis, and dashboard visualization.

The analysis was conducted using Python, PostgreSQL, and Power BI, and the findings were summarized in a report and presentation.

This project demonstrates practical skills required for a Data Analyst role, including data preprocessing, SQL querying, data visualization, and insight generation.

Dataset

The dataset contains 3,900 customer purchase transactions with 18 features describing customer demographics, product details, and purchase behavior.

Key columns include:

Customer ID

Age

Gender

Product Category

Product Name

Quantity Purchased

Purchase Amount

Discount Applied

Review Rating

Subscription Status

Shipping Type

Payment Method

The dataset helps analyze customer behavior, product performance, and revenue patterns.

Tools & Technologies

Python

Pandas

NumPy

Matplotlib / Seaborn

PostgreSQL

SQL for data querying and analysis

Power BI

Interactive dashboard and visualizations

Gamma

Presentation creation

Jupyter Notebook / VS Code

Development environment

Project Steps
1. Data Loading (Python)

Loaded the dataset using Pandas

Checked dataset structure and data types

Generated summary statistics

2. Exploratory Data Analysis (EDA)

Analyzed customer demographics

Studied product categories and revenue trends

Identified purchase patterns

3. Data Cleaning

Handled missing values (e.g., review ratings)

Standardized column names

Removed unnecessary columns

Created additional features such as age groups

4. SQL Analysis (PostgreSQL)

Imported cleaned data into PostgreSQL

Wrote SQL queries to analyze:

Revenue by gender

Product category performance

Discount usage

Customer segmentation

Subscription behavior

5. Dashboard Development (Power BI)

Created an interactive dashboard showing:

Revenue by gender

Sales by product category

Age group revenue distribution

Shipping type comparison

Customer segmentation

6. Reporting & Presentation

Generated a business insights report

Created a presentation using Gamma

Summarized key findings and recommendations

Dashboard

The Power BI dashboard provides a visual overview of:

Total Revenue

Customer Segmentation

Product Performance

Shipping Type Comparison

Age Group Revenue Distribution

The dashboard helps stakeholders quickly understand customer trends and business opportunities.

Key Results

Some important insights from the analysis:

Male customers generated higher total revenue compared to female customers.

Clothing category generated the highest sales.

Jewelry had the highest number of orders in the accessories category.

Only 27% of customers subscribed, indicating potential growth opportunities.

Express shipping customers spent slightly more on average.

Business Recommendations

Increase subscription benefits to improve customer retention.

Implement loyalty programs for repeat buyers.

Optimize discount strategies to balance sales growth and profit margins.

Target marketing campaigns toward high-revenue customer segments.

How to Run the Project
1. Clone the Repository
git clone https://github.com/yourusername/customer-shopping-analysis.git
cd customer-shopping-analysis

2. Install Required Libraries
pip install pandas numpy matplotlib seaborn psycopg2

3. Run Python Analysis

Run the Jupyter Notebook or Python scripts to:

Load the dataset

Perform EDA

Clean the data

4. Import Data into PostgreSQL

Create a table in PostgreSQL

Import the cleaned dataset

Run the provided SQL queries

5. Open Power BI Dashboard

Open the .pbix file in Power BI Desktop to explore the interactive dashboard.

Project Structure
customer-shopping-analysis
│
├── dataset
│   └── Customer_Shopping_Behaviour.csv
│
├── sql
│   └── analysis_queries.sql
│
├── dashboard
│   └── Customer_Shopping_Behaviour.pbix
│
├── presentation
│   └── Customer-Shopping-Behavior-Analysis.pptx
│
└── README.md
