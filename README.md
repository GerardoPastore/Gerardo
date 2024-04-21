# Car Sales Dashboard

### Dashboard Link: Car Sales Dashboard

## Problem Statement

This dashboard is designed to provide insights into car sales performance, enabling effective tracking and analysis of critical key performance indicators (KPIs). By visualizing sales data, it helps in understanding sales trends, identifying opportunities for growth, and making data-driven decisions.

## Steps Followed

- Step 1: Load data into Power BI Desktop: dataset is a csv file.
- Step 2: Data Quality Check: Utilized Power Query Editor to assess data quality, ensuring consistency and accuracy.                                
    -- we don't have any blank value in this report.--
- Step 3: Also since by default, all the car sold must have Car id, Price, Location, Model and Dealer Name.
- Step 4 : Also since by defaoult we created a new table Date, which rapresent all of the date from the minimum date in the report "car_data" column name "date" : Calendar Table = CALENDAR(MIN(car_data[Date]),MAx(car_data[Date])), in addition in the Table "Calendar Table" we created 3 additional columns "Month = FORMAT('Calendar Table'[Date],"MMMM")"; "Week = WEEKNUM('Calendar Table'[Date])"; "Year = YEAR('Calendar Table'[Date])".
- Step 5 : It was observed that in none of the columns errors & empty values were present except 2 columns named "Engine" and "Model".
- Step 6 : Sales Overview, Calculated Year-to-Date (YTD) Total Sales, Month-to-Date (MTD) Total Sales, Year-over-Year (YOY) Growth, and Difference between YTD Sales and Previous Year-to-Date (PTYD) Sales. 

- Step 7 : Since the data contains various type of data, thus in order to represent KPI and measurements three new visuals were added in the pages and represente the YTD Total Sales, Salses Difference with previuos year and the percentage of it, same for the Price and Cars Sold
- Step 8 : Visual filters (Slicers) were added for four fields named "Body Style", "Dealer Name", "Transmission" & "Engine".
- Step 9 : Two card visuals were added to the canvas, one representing a YTD Sales Weekly Trend & other YTD Cars Sold by Dealer Region.
Using visual level filter from the filters pane, was used basic filtering.
 Step 10 : A two bar charts were also added to the report "Overview", PYTD Total Sales by Body Styles rapresent the previuos year total sales fo the different body style & PYTD Total Sales by Color rapresent Previous Year Total Sales for the different color.
 - Step 11 : A table was Added in "Overview" report named Company wise Sales Trend, where was added the performace per company, with Column "Company", Year To Date Average Price", "Year To date Cars Sold", Year To Date Total Sales", "% Total Grand Year To Date Total Sales".
 - Step 12 : In the report "Detail" was added the table where it's Showing into detail the sales per 
 Car Id;
 Date of sold;
 Customer Name;
 Dealer Name;
 Company;
 Color;
 Model of the Car;
 Total Sales.

## Insights

- **Sales Overview:** Provides a snapshot of sales performance, highlighting trends and variations.
![YTD Total Sales](https://github.com/GerardoPastore/Gerardo/assets/157154758/3838ee37-951d-4e24-b567-e930347a4449)


- **Average Price Analysis:** Offers insights into pricing trends, helping in pricing strategy formulation.
![YTD AVG Price](https://github.com/GerardoPastore/Gerardo/assets/157154758/3fba7c54-c455-470c-b58b-58854f42b4ab)


- **Cars Sold Metrics:** Tracks the number of cars sold over time, indicating demand fluctuations.
![YTD Cars Sold](https://github.com/GerardoPastore/Gerardo/assets/157154758/0693da5f-558f-4e40-838d-d7f8f8569cb8)


## Charts Requirement

1. **YTD Sales Weekly Trend:** Displays a line chart illustrating the weekly trend of YTD sales.
![YTD Sales Weekly Trend](https://github.com/GerardoPastore/Gerardo/assets/157154758/1ea633d9-60fb-4e96-a857-98e19f3e1f6f)


2. **YTD Total Sales by Body Style:** Visualizes the distribution of YTD total sales across different car body styles using a Pie chart.
![PYTD Total Sales By Body Style](https://github.com/GerardoPastore/Gerardo/assets/157154758/5e29ac40-2d0b-492b-9e5d-0c7c5e747888)

3. **YTD Total Sales by Color:** Presents the contribution of various car colors to the YTD total sales through a pie chart.
![PYTD Total Sales by Color](https://github.com/GerardoPastore/Gerardo/assets/157154758/5894b90a-01ac-44d4-bdfe-3f78bf545a38)


4. **YTD Cars Sold by Dealer Region:** Showcases the YTD sales data based on different dealer regions using a map chart.
![YTD Cars Sold by Dealer Region](https://github.com/GerardoPastore/Gerardo/assets/157154758/2ef99c5e-c4df-443c-ad8b-6bb15935530a)


5. **Company-Wise Sales Trend in Grid Form:** Provides a tabular grid displaying the sales trend for each company.
![Company-Wise Sales Trend in Grid Form](https://github.com/GerardoPastore/Gerardo/assets/157154758/705b46cc-9b4d-4fdb-b0e3-5cacf517ba01)


6. **Details Grid Showing All Car Sales Information:** Presents all relevant information for each car sale, including model, body style, color, sales amount, dealer region, and date.
![Details Grid Showing All Car Sales Information](https://github.com/GerardoPastore/Gerardo/assets/157154758/918c81ef-fbde-4dd3-9e71-6fb458e19b88)
