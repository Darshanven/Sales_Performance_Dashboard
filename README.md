\# Sales Performance Dashboard



\## Project Overview



The Sales Performance Dashboard is a data analytics project designed to analyze sales, profit, customers, products, regions, and business performance using a real-world retail sales dataset.



The project combines Python-based data analysis with an interactive Power BI dashboard to identify sales trends, profitable products, high-performing regions, and areas that require business improvement.



\## Objectives



\* Analyze overall sales and profit performance

\* Identify top-performing products and categories

\* Analyze sales performance across regions and states

\* Understand customer purchasing behavior

\* Identify profitable and loss-making products

\* Analyze monthly and yearly sales trends

\* Create an interactive business dashboard

\* Generate actionable business insights



\## Dataset



The project uses the Superstore Sales Dataset.



The dataset contains information about:



\* Orders

\* Customers

\* Products

\* Categories

\* Sub-Categories

\* Sales

\* Quantity

\* Discount

\* Profit

\* Regions

\* States

\* Cities

\* Order Dates

\* Ship Dates

\* Shipping Modes



\## Technologies Used



\* Python

\* Jupyter Notebook

\* Pandas

\* NumPy

\* Matplotlib

\* Seaborn

\* Scikit-learn

\* Power BI

\* Microsoft Excel

\* Git

\* GitHub



\## Project Workflow



```text

Dataset

&#x20;  ↓

Data Collection

&#x20;  ↓

Data Cleaning

&#x20;  ↓

Exploratory Data Analysis

&#x20;  ↓

Data Visualization

&#x20;  ↓

Business Analysis

&#x20;  ↓

Power BI Dashboard

&#x20;  ↓

Business Insights

&#x20;  ↓

GitHub Documentation

```



\## Project Structure



```text

Sales-Performance-Dashboard/

│

├── Dataset/

│   └── SampleSuperstore.csv

│

├── Notebook/

│   └── Sales\_Performance\_Analysis.ipynb

│

├── Dashboard/

│   └── Sales\_Performance\_Dashboard.pbix

│

├── Reports/

│   └── Business\_Insights\_Report.pdf

│

├── README.md

```



\## Data Cleaning



The dataset was cleaned and prepared before performing analysis.



Main data preprocessing steps included:



\* Loading the dataset using Pandas

\* Checking dataset dimensions

\* Checking data types

\* Identifying missing values

\* Removing duplicate records

\* Converting date columns into datetime format

\* Checking numerical columns for invalid values

\* Creating additional analytical columns

\* Preparing the dataset for visualization



Example Python code:



```python

import pandas as pd

import numpy as np



df = pd.read\_csv("Dataset/SampleSuperstore.csv")



print(df.shape)

print(df.head())

print(df.info())

print(df.isnull().sum())

print(df.duplicated().sum())

```



\## Exploratory Data Analysis



The project analyzes the dataset from multiple business perspectives.



\### Key Metrics



The dashboard focuses on:



\* Total Sales

\* Total Profit

\* Total Orders

\* Total Quantity Sold

\* Total Customers

\* Average Order Value

\* Profit Margin



\### Sales Analysis



Sales performance was analyzed based on:



\* Year

\* Month

\* Category

\* Sub-Category

\* Region

\* State

\* Customer Segment



\### Profit Analysis



Profitability was analyzed to identify:



\* Most profitable categories

\* Most profitable products

\* Loss-making products

\* Regional profitability

\* Impact of discounts on profit



\## Data Visualization



Python visualizations were created to understand business trends.



Examples include:



\* Monthly sales trend

\* Category-wise sales

\* Category-wise profit

\* Regional sales

\* Regional profit

\* Top products

\* Bottom products

\* Sales by customer segment

\* Discount vs profit analysis



Example:



```python

import matplotlib.pyplot as plt

import seaborn as sns



plt.figure(figsize=(10, 5))



sns.barplot(

&#x20;   data=df,

&#x20;   x="Category",

&#x20;   y="Sales",

&#x20;   estimator=sum

)



plt.title("Sales by Category")

plt.xlabel("Category")

plt.ylabel("Sales")



plt.show()

```



\## Power BI Dashboard



The Power BI dashboard provides an interactive view of the company's sales performance.



\### Dashboard Sections



The dashboard includes:



\* Sales KPI

\* Profit KPI

\* Orders KPI

\* Quantity KPI

\* Profit Margin KPI

\* Sales trend

\* Profit trend

\* Category analysis

\* Regional analysis

\* Customer segment analysis

\* Top products

\* Bottom products

\* Interactive filters



\### Filters



Users can filter the dashboard using:



\* Year

\* Region

\* State

\* Category

\* Sub-Category

\* Segment

\* Ship Mode



\## Dashboard Preview



Add your dashboard screenshot here:



```text

!\[Sales Performance Dashboard](Images/dashboard.png)

```



\## Key Business Insights



The analysis helps identify several important business patterns.



\### Sales Performance



\* Sales performance varies across regions and customer segments.

\* Technology and Furniture contribute significantly to overall sales.

\* Consumer customers represent an important portion of total sales.



\### Profitability



\* High sales do not always result in high profit.

\* Some products generate low or negative profit because of high discounts.

\* Discount levels have a noticeable relationship with profitability.



\### Regional Performance



\* Some regions generate stronger sales and profit than others.

\* Regional analysis helps identify markets requiring additional attention.



\### Product Performance



\* A small group of products contributes significantly to total sales.

\* Some products have high sales but weak profitability.

\* Low-performing products require pricing or discount strategy review.



\## Business Recommendations



Based on the analysis, the following strategies are recommended:



1\. Reduce excessive discounts on products with low profit margins.



2\. Focus marketing efforts on high-value customer segments.



3\. Promote highly profitable products along with high-demand products.



4\. Review loss-making products and evaluate their pricing.



5\. Strengthen sales strategies in regions with strong growth potential.



6\. Monitor monthly sales trends to support inventory planning.



7\. Use customer and product performance data to create targeted marketing campaigns.



\## Expected Business Benefits



The dashboard helps businesses:



\* Monitor sales performance

\* Track profitability

\* Identify growth opportunities

\* Improve pricing decisions

\* Optimize discount strategies

\* Understand customer segments

\* Identify high-performing products

\* Support data-driven decision making



\## How to Run the Project



\### 1. Clone the Repository



```bash

git clone https://github.com/Darshanven/Sales_Performance_Dashboard.git

```



\### 2. Open the Project



```bash

cd Sales-Performance-Dashboard

```



\### 3. Install Required Libraries



```bash

pip install pandas numpy matplotlib seaborn scikit-learn jupyter

```



\### 4. Start Jupyter Notebook



```bash

jupyter notebook

```



Open:



```text

Notebook/Sales\_Performance\_Analysis.ipynb

```



\### 5. Run the Notebook



Run the notebook cells sequentially to perform:



\* Data loading

\* Data cleaning

\* Exploratory analysis

\* Visualization

\* Business analysis



\### 6. Open the Power BI Dashboard



Open:



```text

Dashboard/Sales\_Performance\_Dashboard.pbix

```



in Microsoft Power BI Desktop.



\## Requirements



Create a `requirements.txt` file containing:



```text

pandas

numpy

matplotlib

seaborn

scikit-learn

jupyter

openpyxl

```



Install all dependencies using:



```bash

pip install -r requirements.txt

```



\## Project Deliverables



\* Python/Jupyter Notebook

\* Cleaned dataset

\* Exploratory Data Analysis

\* Data visualizations

\* Power BI dashboard

\* Business insights report

\* GitHub repository

\* Project documentation



\## Future Improvements



Future versions of the project can include:



\* Real-time sales data

\* Customer segmentation using RFM analysis

\* Sales forecasting

\* Machine learning-based prediction

\* Automated dashboard updates

\* Customer churn prediction

\* Product recommendation system

\* Deployment as a web application



\## Author



Darshan Venkatesh Daivadnya



Data Science Student

Moodlakatte Institute of Technology, Kundapura



\## Project Type



Data Analytics | Business Intelligence | Data Visualization



\## Internship Project



This project was developed as part of a Data Analytics Internship project at Kinetrexa Software Private Limited.



"# Sales_Performance_Dashboard" 
