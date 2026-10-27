
## 📊 Customer Sales Exploratory Data Analysis (EDA)

An exploratory data analysis project using Python to analyze customer purchasing behavior, identify sales trends, evaluate customer segments, and generate actionable business insights.

### 📌 Project Overview


This project was completed during my internship at Swynex Technologies. Initially, I was assigned a customer sales dataset for data cleaning. After completing the cleaning task, I was asked to perform Exploratory Data Analysis (EDA) on the same dataset.

I inspected the dataset again, addressed additional data-quality issues, calculated key performance indicators (KPIs), and created visualizations to understand customer purchasing patterns and sales trends.

The project demonstrates how Python-based data analysis can help transform raw customer data into meaningful business insights.

### 🎯 Project Objectives

Clean and prepare the customer sales dataset for analysis.

Identify and handle missing, invalid, and inconsistent values.

Calculate key performance indicators related to customers, purchase amounts, and feedback.

Analyze purchase amounts across gender and age groups.

Examine monthly purchase trends.

Explore correlations between numerical variables.

Generate business insights and recommendations based on the analysis.

### 🛠️ Tools and Technologies

Python – Data analysis and processing

Pandas – Data manipulation and cleaning

NumPy – Numerical operations

Matplotlib – Data visualization

Seaborn – Statistical visualization

Jupyter Notebook – Interactive analysis and documentation

### 📂 Dataset Information

Attribute	Details  

Dataset Name	Customer Sales Dataset

Original Dataset Size	10,127 records

Total Columns	12

Project Type	Data Cleaning, EDA & Business Analytics

Internship Organization	Swynex Technologies

The dataset contains customer-related information, including age, gender, purchase amount, last purchase date, and feedback score.

Note: The original dataset contains 10,127 records. The KPI calculations identify 9,001 customers; this count should be interpreted according to the customer-counting method used in the notebook.

🔄 Project Workflow

Data Inspection – Examined the dataset using head(), shape, info(), and describe().

Data Cleaning – Handled invalid ages, missing values, inconsistent gender labels, and negative purchase amounts.

Data Transformation – Converted columns to appropriate data types and created age groups.

KPI Calculation – Calculated total customers, total purchase amount, average purchase amount, and average feedback score.

Exploratory Data Analysis – Investigated purchasing patterns across demographic groups and months.

Data Visualization – Created charts to communicate the findings.

Business Insights – Interpreted the results and developed recommendations.

📈 Key Performance Indicators (KPIs)

The following KPIs were calculated during the analysis:

KPI	Value

Total Customers	9,001

Total Purchase Amount	265,295,613

Average Purchase Amount	26,196.86

Average Feedback Score	5.0

KPI Insights

Total Customers: The customer count used in the KPI calculation was 9,001.

Total Purchase Amount: The aggregate recorded purchase amount was 265,295,613.

Average Purchase Amount: The calculated average purchase amount was 26,196.86.

Average Feedback Score: The average feedback score was 5.0. The feedback scale and score distribution should be checked when interpreting this result.

### 🔍 Business Problems and Key Findings

#### 1. How are purchase amounts distributed across gender categories?

Findings:

Male customers contributed approximately 46.2% of recorded purchase amounts.

Female customers contributed approximately 45.1%.

The Unknown category contributed approximately 8.6%.

Business Insight: Male and female categories contributed similar proportions of recorded purchase amounts. Improving missing or unknown gender information could support more reliable demographic analysis.

#### 2. Which age groups contribute the highest purchase amounts?

Findings:

The 45–60 age group had the highest total purchase amount in the displayed chart.

The 0–18 age group had the lowest total purchase amount.

Middle-aged groups contributed more than the youngest group.

Business Insight: Customers aged 30–60 may be valuable segments for further investigation. Customer counts and average purchase amounts should also be compared to distinguish segment size from individual spending behavior.

#### 3. How do purchase amounts change month by month?

Findings:

A sharp increase was observed in March 2025.  

Another prominent increase occurred in July 2025.

Purchase amounts declined after July through September.

October 2025 showed a substantial decrease compared with September.

Business Insight: These changes warrant further investigation to determine whether they reflect genuine purchasing patterns, incomplete reporting periods, or unusual records.

#### 4. Is customer age related to purchase amount?

Finding:

The correlation between Age and Purchase_Amount was approximately 0.02.

Business Insight: The analysis showed almost no linear relationship between age and purchase amount. Other customer characteristics may provide additional insights into spending behavior.

#### 5. Is customer feedback related to purchase amount?

Finding:

The correlation between Feedback_Score and Purchase_Amount was close to zero.

Business Insight: No meaningful linear relationship was identified in this analysis. Additional investigation would be required to assess whether customer feedback is associated with purchasing behavior in other ways.

#### 6. Are there data-quality issues affecting the analysis?

Findings:

Invalid age entries included Unknown, -10, and 250. 

Gender values contained inconsistent formatting.

The Last_Purchase_Date column contained 1,009 missing values.

Four records contained negative purchase amounts.

The maximum purchase amount was 9,999,999 and requires verification.

Business Insight: Data validation and consistent cleaning rules are essential for reliable reporting and business decision-making.

## 📊 Visualizations

Four visualizations were created using Matplotlib and Seaborn.

1. Sales Distribution by Gender

A pie chart comparing the percentage contribution of each gender category to total recorded purchase amounts.

2. Sales Distribution by Age Group

A bar chart comparing total purchase amounts across different age groups.

3. Monthly Purchase Trends

A line chart showing purchase amounts by recorded last-purchase month from October 2024 to October 2025.

4. Customer Data Correlation Heatmap

A heatmap illustrating linear correlations between selected numerical variables.

Repository note: Add your exported chart images to a folder such as images/ and embed them below if you want the visualizations to appear directly on GitHub.

Example:

markdown
![Sales Distribution by Gender]

## 💡 Business Recommendations

Improve Data Quality: Introduce validation rules for ages, dates, gender categories, and purchase amounts.

Investigate Unusual Values: Verify negative purchase amounts and the unusually large purchase amount before drawing conclusions.

Improve Customer Segmentation: Compare customer counts, total purchase amounts, and average purchase amounts across age groups and gender categories.

Monitor Monthly Trends: Investigate the March and July peaks and October decline while checking reporting completeness.

Improve Customer Insights: Explore repeat purchases, retention, feedback patterns, and geographic performance if suitable data becomes available.

Improve Correlation Analysis: Exclude phone numbers and other identifier columns from numerical correlation analysis.

Track KPIs Regularly: Monitor customer counts, total purchase amounts, average purchase amounts, and feedback scores over time.

## 📁 Suggested Repository Structure

Organize your GitHub repository using the following structure:

text
Customer-Sales-EDA/

│

├── README.md

├── customer_sales_eda.ipynb

├── data/

│   └── README.md

├── images/

│   ├── sales_by_gender.png

│   ├── sales_by_age_group.png

│   ├── monthly_purchase_trends.png

│   └── correlation_heatmap.png

└── requirements.txt


README.md – Project documentation.

customer_sales_eda.ipynb – Jupyter Notebook containing the analysis.

data/ – Dataset directory, if sharing the data is permitted.

images/ – Exported charts and visualizations.

requirements.txt – Python library dependencies.

⚙️ How to Run This Project

Prerequisites

Install Python and Jupyter Notebook, or use an environment such as JupyterLab or Google Colab.

1. Clone the repository

bash

git clone https://github.com/YOUR-USERNAME/Customer-Sales-EDA.git


Replace YOUR-USERNAME with your GitHub username.

2. Navigate to the project directory

bash

cd Customer-Sales-EDA

3. Install the required libraries

bash

pip install pandas numpy matplotlib seaborn jupyter
48. Launch Jupyter Notebook

bash

jupyter notebook


Open customer_sales_eda.ipynb and run the notebook cells in order.

Note: Update the notebook's dataset path to match your local file location.

📦 Requirements

You can create a requirements.txt file containing:

text

pandas

numpy

matplotlib

seaborn

jupyter


Install all dependencies using:

bash

pip install -r requirements.txt

📚 Skills Demonstrated

Data Cleaning and Preprocessing

Exploratory Data Analysis (EDA)

Missing Value Handling

Data Type Conversion

Feature Engineering and Age Grouping
KPI Calculation

GroupBy Aggregation

Correlation Analysis

Data Visualization

Statistical Interpretation

Business Insight Generation

## 🏁 Conclusion

This project strengthened my practical skills in Python-based data cleaning, exploratory data analysis, KPI calculation, data visualization, and business analytics during my internship at Swynex Technologies.

The analysis highlighted differences in purchase amount contributions across demographic categories, variations in monthly purchase amounts, and data-quality issues that require attention. It also demonstrated that age and feedback score had little linear correlation with purchase amount in the analyzed dataset.

The project shows how data analysis can support more informed business decisions by identifying patterns, monitoring KPIs, and highlighting areas for further investigation.

## 👨‍💻 Author

Shubham Lokhande

Data Analyst Intern

Internship Organization: Swynex Technologies


<img width="612" height="307" alt="Customer_Sales_Exploratory_Data_Analysis" src="https://github.com/user-attachments/assets/06c9c528-c5f6-4ec2-8b52-d0b5523e3639" />




