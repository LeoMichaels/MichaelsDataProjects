# GPL_Cloud Billing Dashboard Project 2

### Dashboard Link : https://app.powerbi.com/links/FSbe1kDYeS?ctid=8acbc2c5-c8ed-42c7-8169-ba438a0dbe2f&pbi_source=linkShare

## Problem Statement

This dashboard helps the airlines understand their Cloud Service costs better. It helps the stakeholders know which Cloud services are more efficient than others. Through a metric of time-value utilisation that factors CPU & Memory Utilisation along with Total Network traffic divided by Total Costs and Durations of operations, which services must be maximised and those minimised are the two primary objectives.


### Steps followed 

- Step 1 : Loaded data to Python Jupyter for analysis using pandas and numpy.

- Step 2 : Preprocessed data and engineered new features to calculate duration(hours) based on given start and end dates, total network traffic

- Step 3 : Calculated time-value utility as sum of utilisation and network traffic dvided by costs and durations of service usage.

- Step 4 : Grouped by service name calculating the median time_value_utility for each group, and using pd.qcut to classify groups into High, Medium, and Low efficiency accordingly.

- Step 5 : Load data into Power BI Desktop, dataset is an Excel file modified by Python Pandas and conditional masks. 

- Step 6 : Installed a stacked bar chart + line-chart tempmlate and loaded the Services under the X-Axis and total responses under the Y-Axis, and total costs plotted on the secondary y-axis line. 

- Step 7 : Colour coded High, Medium, Low efficiency service requests to illustrate overall efficiency of a service.

- Step 8 : Repeated preceeding steps for both inefficient and efficient services and regions.

- Step 9 : Verified data used to count response requests, formatting canvas to fit visuals, colour coding high to low priority statistics.

- Step 10 : A bar chart was also added to the report design area representing the number of satisfied & neutral/unsatisfied customers. While creating this visual, field named "Gender" was also added to the Legends bucket, thus number of customers are also seggregated according the gender. 



# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Services to minimise usage:
-- Expenditure to inefficiency comparison reveals: 
1. Cloud Build
2. Pub/Sub
3. Cloud CDN
4. Cloud Interconnect
5. Cloud Endpoints

-- are highly inefficient and have higher associated costs.

### [2] Services to maximise:
-- In the Expenditure to efficiency comparison plot:
1. Compute Engine
2. AI platforms
3. Cloud Run
4. Cloud Functions
5. Kubernetes Engine
6. DataFlow have lower associated costs but higher efficiencies.

-- are efficient although with relatively lower associated usage.

In summary this dashboard summarised services to maximise and minimise utility of based on an efficiency metric and a stacked-bar-chart + secondary y-axis line-plot analysis.

# For further improvement:
Further calculations of how inefficient each metric has been as opposed to visual comparisons. For example Cloud Memorystore has an XYZ inefficienc compared to Firestore. The data is available to make such a calculation and thus requires its own datacard on the dashboard to further support the points made by the dashboard.
