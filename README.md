# Medical-Insights-Dashboard
Developed interactive Power BI dashboard by transforming and modeling inpatient and outpatient data, delivering detailed insights through dynamic visualizations.

[Access the Dashboard Online](https://app.powerbi.com/view?r=eyJrIjoiMDU4Y2YwMzUtY2MwMS00OWI2LWIyMWQtZTIyYjY3M2I2ZDA1IiwidCI6ImI0MmFhYTY2LTA2NWMtNDE2NS05MGE3LTgwMjIyMmViY2U1MSJ9&embedImagePlaceholder=true)  

## Project Overview 
This project is developed using Power BI, leveraging Power Query for data transformation and DAX for creating calculated fields and measures. The dashboard integrates inpatient and outpatient data, offering a comprehensive view of healthcare metrics. With a focus on data accuracy, the report provides dynamic visualizations that allow users to explore key insights interactively. Features such as slicers, custom tooltips enable detailed drilldowns and data exploration, ensuring meaningful insights into healthcare performance. The dashboard is designed for user interactivity, allowing both high-level summaries and detailed views for in-depth analysis. 

## How to Use 
1. Clone the repository and download the Power BI file. 

2. Open the .pbix file in Power BI Desktop. 

3. Ensure the data sources are correctly linked. 

4. Explore the report pages including the dashboard page 

5. Interact with slicers and tooltips to gain insights. 

6. Publish to Power BI Service if needed. 

[Access the Dashboard Online](https://app.powerbi.com/view?r=eyJrIjoiMDU4Y2YwMzUtY2MwMS00OWI2LWIyMWQtZTIyYjY3M2I2ZDA1IiwidCI6ImI0MmFhYTY2LTA2NWMtNDE2NS05MGE3LTgwMjIyMmViY2U1MSJ9&embedImagePlaceholder=true) 

## Steps to Build the Dashboards

### 1. Requirement Gathering
- Defined the objectives and goals of the dashboard.
- Understood the available data and its structure.

### 2. Data Collection
- Loaded data from two folders: **Inpatient** and **Outpatient**.
- Each folder contained four **CSV** files with data from the years 2018, 2019, 2020, and 2021.
- The files contained monthly patient details entered at the end of each month.

### 3. Data Transformation and Modeling

#### In Power Query Editor:
- Checked and changed data types.
- Renamed headers for better readability and easier modeling.
- Added a missing **Case_Type** field in the **Outpatient** table, filling it with ‘Outpatient’.
- Reordered fields to maintain consistency across tables.
- Merged the **Inpatient** and **Outpatient** datasets by appending queries, renaming the merged dataset as ‘All_Data’.
- Identified and corrected typographical errors and improper spacing issues.
- Replaced blank values with ‘No Input’ and ‘null’ where appropriate.
- Applied all transformations and loaded the data.

#### In Model View:
- Hid the **Inpatient** and **Outpatient** tables from the report view.
- Loaded a separate **CSV** file containing **specialty groups** to categorize specialties.
- Created a relationship between the **specialty group** table and **All_Data**.

### 4. Data Visualization
- Created a blueprint for dashboards: **Summary**, **Detailed View**, and **Drilldown**.
- Used various visualizations, including **cards**, **charts**, and **tables**.
- Implemented **DAX** functions in cards to display last month’s details.
- Calculated **average** and **median** values using **DAX measures**.
- Created an interactive slicer with buttons (**Average/Median**) by generating a table containing the values ‘Average’ and ‘Median’.
- Assigned a **DAX measure** to each visualization to allow switching between average and median.
- Created a dynamic title using **DAX** to indicate whether the dashboard is showing average or median values.
- Adjusted visual interactions using **Edit Interactions** and additional **DAX measures**.
- Developed a **Detailed View** page with tabular data and slicers.
- Added a **navigation info button** on the Summary dashboard for easy access to the Detailed View.
- Created a **Drilldown** page displaying the top 10 specialty groups based on total values, with appropriate formatting.
- Designed a **custom tooltip**: assigned the **Drilldown** page as a tooltip for charts in the Summary dashboard, allowing users to hover over a chart to view detailed drill-down data.
- Hid the **Drilldown** page from direct navigation.

### 5. Publishing
- Published the report to **Power BI Service**.
- Pinned the report to the dashboard.
- Downloaded the **Power BI report** file for future use.
- Published to web so that users can view and interact via the link generated.  
  [Access the Dashboard Online](https://app.powerbi.com/view?r=eyJrIjoiMDU4Y2YwMzUtY2MwMS00OWI2LWIyMWQtZTIyYjY3M2I2ZDA1IiwidCI6ImI0MmFhYTY2LTA2NWMtNDE2NS05MGE3LTgwMjIyMmViY2U1MSJ9&embedImagePlaceholder=true) 
