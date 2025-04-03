# GPL_Cloud Billing Practice [Project-1]

### Dashboard Link : https://app.powerbi.com/links/FSbe1kDYeS?ctid=8acbc2c5-c8ed-42c7-8169-ba438a0dbe2f&pbi_source=linkShare

## Problem Statement

This dashboard helps the stakeholder of the dataset understand their Cloud Service costs better. It helps the stakeholders know which Cloud services are more efficient than others. Through a metric of time-value utilisation that factors CPU & Memory Utilisation along with Total Network traffic divided by Total Costs and Durations of operations, which services must be maximised and those minimised are the two primary objectives.


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

- Step 10 : Final review of calculations and data fields used in graphs, and published.


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
6. DataFlow

-- are efficient although with relatively lower associated usage.

In summary this dashboard summarised services to maximise and minimise utility of based on an efficiency metric and a stacked-bar-chart + secondary y-axis line-plot analysis.

# For further improvement:
Further calculations of how inefficient each service or region has been as opposed to visual comparisons. More exploration on regional-differences in utilisation should have been expanded on. For example Cloud Memorystore has an XYZ inefficienc compared to Firestore. The data is available to make such a calculation and thus requires its own datacard on the dashboard to further support the points made by the dashboard.


<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />

# Tunisian-Property-Prices Practice-Project_02

### Dashboard Link : https://app.powerbi.com/links/DlBxz-2948?ctid=8acbc2c5-c8ed-42c7-8169-ba438a0dbe2f&pbi_source=linkShare

## Problem Statement

This dashboard helps the stakeholder understand the property prices of different property types across the cities. There are n-number of properties in French script, some for Rent or Lease, with given parameters on size and cost.

Objectives are to:
1. Identify which cities are ideal for which type of property
2. Identify where prices are higher for which type of property


### Steps followed 

- Step 1 : Load data into Python
- Step 2 : Retrieved translation for Category and Type fields
- Step 3 : Replaced all French script with English version
- Step 4 : Corrected unformatted accented French script with neutral English letters to simplify analysis.
- Step 5 : Replaced (-1) parameters that according to the dataset owner represent Null values, with np.Nans null values.
- Step 6 : Calculated the price per meter square as the division of the given logarithmic price over the property's size.
- Step 7 : Data is grouped by city, region and category, with aggregates of the price per meter square mean and medians and total number of properties under each category.
- Step 8 : The price is used to classify the group into labels of low to medium and to high based on quantile distribution.
- Step 9 : The modified excel book is loaded into PowerBI
- Step 10 : Stacked bar charts are iteratively created for each property type (Apartments, FLatshare, Holiday Rentals, etc.) with color coded classification of high to low property prices.
- Step 11 : Step 10 is repeated for exclusively high and low price properties per category.

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard:

### [1] Cities with favourable pricing inferred from descending order of stacked-bar chart

Favourable - Higher count of Low-Price-Class properties

Unfavourable - Higher counts of High or Medium - Price-Class properties

1. Apartments
* Gafsa (Favourable)
* Kasserine (Favourable)
* Medenine (Favourable)

2. Flatshares
* Tunis (Favourable)
* Ariana (Favourable)
* Ben Arous (Unfavourable)

3. Holiday Rentals
* Sousse (Favourable)
* Gabes (Favourable)
* Nabeul (Favourable)

4. House and Villas
* Tunis (Favourable)
* Sfax (Favourable)
* Sousse (Favourable)
* Ariana (Favourable)

5. Office and Office Floor properties
* Tunis (Favourable)
* Ariana (Favourable)

6. Shops and Industrial Properties:
* Monastir (Favourable)
* Sfax (Favourable)
* Sousse (Favourable)
