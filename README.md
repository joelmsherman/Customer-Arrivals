# Hours of Operation Truncation and Customer Impacts Analysis
![image](https://github.com/joelmsherman/Customer-Arrivals/blob/master/Images/image.jpg)

## Background
Widget Inc sells a variety of consumer products to hundreds of customers in several store locations in the Portland metropolitan region.  Widgets hours of operation for two of its locations are generous to early morning and late evening customers, but as a result, have dramatically increased operating costs.  Widget's operations team would like to assess the effect of truncating store hours on its customers, but relevant data is only available in excel spreadsheets that are prepared periodically by company analysts.   

## Objective
This analysis seeks to answer Widget's primary questions about hours of operation truncation on customers, but also provide management with a robust, scaleable, interactive report on company sales that is directly connected to the company's point of sales system.

## Methods
The analysis is conducted in the following steps.

### Data Extraction and Prep
Widget's point of sale system is a SQL Server database.  Relevant data was extracted, shaped and landed into a company on-prem data warehouse.  The data is materialized hourly.  The data was tested for veracity against existing excel spreadsheets to validate the ETL logic.

### Data Analysis
To answer Widget's questions about hours of operation truncation and customer impacts, [an interactive notebook](https://app.hex.tech/5b266aaf-b343-4ae7-bdea-218e8fe3001f/app/ca32cac7-d980-4b41-819c-800d6dda88c9/latest) was developed.  This notebook is directly connected to Widget's data warehouse and available on-demand by the Widget's operations team.  

## Results
The analysis shows a clear peak in Widget's sales in the middle of the day, with far fewer sales in the early morning and later afternoons.  For those lower sales hours, Widget can view the sales of specific customers over time to determine which customers would see the greatest impacts from truncating those hours.

## Value Proposition
Widgets operating costs are significantly higher at two of its store locations due to extended hours of operation that have been in effect since opening.  While some of Widget's customers appear to do the bulk of their business during these hours, most do not.  Although an in-depth financial analysis was not part of the scope, Widget can be confident that hours of operation truncation would only impact a few of its customers, while saving significant costs.  