# bank-
Analysis of customers and products of the store using Python and Power BI.
 Project Overview
This project applies Exploratory Data Analysis (EDA) and Data Storytelling to optimize the business performance of a global retail chain. By integrating Python for deep statistical exploration and Power BI for interactive reporting, the project identifies a "Growth Paradox"—where increasing revenue does not always lead to higher profitability due to rising operational costs
. The goal is to move from descriptive "what happened" analytics to prescriptive "how to improve" strategies
.
 Dataset Description
The analysis utilizes a relational data model consisting of four primary tables
:
Fact_Sales: Core transactional data including Revenue_VND, COGS_VND, Quantity, and SalesDate
.
Fact_Expense: Time-varying operational costs such as Salaries, Marketing, and Logistics
.
DimCustomer: Classification of major clients across 3 Regions (North, Central, South) and 3 Segments (Retail, SMB, Enterprise) [2, DimCustomer.csv].
DimProduct: Product catalog including categories like Electronics, Food, and Materials
.
 Tools & Technologies
Python: Used for data cleaning, transformation, and multivariate statistical analysis.
Libraries: Pandas (ETL), Plotly (3D interactive plots), Seaborn/Matplotlib (Statistical distributions)
.
Power BI: Used for building a Decision Support System (DSS) with interactive dashboards, DAX measures, and drill-down features
.
 Project Workflow
The project follows a rigorous 8-step data science lifecycle
:
Analytical Mapping: Defining business questions regarding profit margins and regional efficiency
.
Data Gathering & Preparation: Loading CSV files and merging tables in Python to create a unified df_final
.
Data Cleaning: Imputing missing COGS_VND values using central tendency measures (Mean) and normalizing financial attributes
.
Descriptive Analysis: Calculating Mean, Median, and Standard Deviation to understand sales distributions
.
Multivariate Visualization: Implementing 3D Scatter Plots to correlate Revenue, COGS, and Quantity [62, Python Code history].
Data Storytelling: Constructing a narrative focused on the Enterprise segment as the "profit backbone"
.
Dashboard Development: Designing a Power BI interface with slicers for Year, Region, and Segment
.
Presentation: Synthesizing findings to recommend a 15% marketing budget reallocation.
 Python EDA & Visuals
Correlation Analysis: Used Pearson Correlation (PCC) to find the relationship between Marketing spend and Revenue
.
Multivariate 3D Plots: Leveraged Plotly to visualize 5 dimensions simultaneously (Revenue, COGS, Quantity, Segment, and Region) to detect financial clusters and outliers
.
Outlier Detection: Used Boxplots to identify "super orders" that significantly skew average performance
.
 Power BI Dashboard
The interactive dashboard features
:
KPI Cards: Real-time tracking of Total Sales (>262B VND) and Gross Profit Margin (~29.35%) [Conversation history].
Treemaps: Visualizing profit contribution by product category (e.g., Electronics vs. Food)
.
Time-Series Trends: Monthly sales volume analysis to identify seasonal peaks
.
Interactivity: Full Drill-down from Category to specific Product IDs and Tooltips for detailed hover information
.
 Key Insights
The Growth Paradox: The North region generates the highest revenue but has lower net margins due to inefficient Logistics allocation [Conversation history].
Strategic Backbone: The Enterprise segment contributes the highest Average Order Value (AOV) and is vital for long-term profit stability
.
Efficiency Target: The overall margin of 29.35% is just below the 30% strategic goal, highlighting a need for cost optimization in high-volume Retail segments [Conversation history].
📥 How to Run
Python: Open the Jupyter Notebook and run all cells to perform the data transformation and generate EDA plots.
Power BI: Open the .pbix file to interact with the final dashboard. Ensure the data source paths are updated to your local directory.
