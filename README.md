# Coffee Sales Dashboard

## Project Overview

This dashboard will enable users to quickly identify trends in coffee bean sales and make comparisons across different bean types and countries. This project involves end-to-end data analysis in Excel, from data gathering to data cleaning and transformation, all the way to creating meaningful visualizations in the form of a dynamic and interactive dashboard.

<img width="1353" alt="Overview of Coffee Sales Dashboard" src="https://github.com/fangoaish/Excel__Coffee-Sales-Dashboard/assets/51399519/f53cc2bf-279b-4256-b2b9-658a1012cabd">


## Project Steps
1. Data Gathering
2. Data Preparation Using Advanced Formulas and Functions
3. Exploratory Data Analysis
4. Data Visualizations and Dashboard Build Using **Pivot Tables**, **Pivot Charts**, **Timeline** and **Slicers**

## Data Sources
The data source is a fictitious coffee bean sales dataset provided by Mo Chen. Link [HERE](https://github.com/mochen862/excel-project-coffee-sales). 
  - coffeeOrderData.xlsx

The data contains three separate tables:
- **orders**, **customers** and **products**
  - The **orders** table is the _fact table_
  - The **customers** and **products** tables are the _dimension tables_.

  
## Data Preparation
- Use **XLOOKUP** to look up the full customer name from the _customers_ table to the _orders_ table
  
<img width="725" alt="XLookup - Customer Name" src="https://github.com/fangoaish/Excel__Coffee-Sales-Dashboard/assets/51399519/c7e1ab19-0966-4890-bbe8-0feadbfabdf7">

- Use **IF** and **XLOOKUP** to look up the email address from the _customers_ table to the _orders_ table
  
<img width="1431" alt="IF    XLookup - email address" src="https://github.com/fangoaish/Excel__Coffee-Sales-Dashboard/assets/51399519/19d3c6ca-148c-47f1-9de4-122bf70cea37">


- Use **XLOOKUP** to look up the country of the customer from the _customers_ table to the orders table
<img width="1087" alt="XLookup Country" src="https://github.com/fangoaish/Excel__Coffee-Sales-Dashboard/assets/51399519/b364b778-faa5-4a84-86f8-87d6e27134aa">


- Use only one dynamic **INDEX MATCH** formula to look up the coffee type, roast type, size and unit price values from the _products_ table to the _orders_ table.
- Use the correct cell locking (i.e. “$” signs) so that the formula in cell H1 can be automatically filled to the right and to the bottom of the table.
<img width="1191" alt="Index Match - Coffee Type, Roast Type, Size and Unite Price" src="https://github.com/fangoaish/Excel__Coffee-Sales-Dashboard/assets/51399519/f26dca47-5673-4756-a8ca-f34d400ac434">


- Calculate the sales as the product of **price*quantity**
<img width="1055" alt="Sales Calculation" src="https://github.com/fangoaish/Excel__Coffee-Sales-Dashboard/assets/51399519/d02bdd82-8fce-4ba5-95ed-95b04a33ca68">


- Use multiple **IF** functions to map the full coffee type and roast type names
<img width="1184" alt="Multiple IF - Coffee Type" src="https://github.com/fangoaish/Excel__Coffee-Sales-Dashboard/assets/51399519/c01f3cb0-f322-4e52-b315-1ac66bdcd9ba">
<img width="1259" alt="Multiple IF - Roast Type" src="https://github.com/fangoaish/Excel__Coffee-Sales-Dashboard/assets/51399519/b542926e-0ce6-4695-82f5-987a254f71c9">


- Use **XLOOKUP** to look up the loyalty card status from the _customers_ table to the _orders_ table
<img width="1314" alt="'XLookup - Loyalty Card" src="https://github.com/fangoaish/Excel__Coffee-Sales-Dashboard/assets/51399519/c5ceb6cb-f66d-45c6-9084-444797926034">


## Exploratory Data Analysis
The primary objective of the Coffee Sales Dashboard is to provide comprehensive insights into our coffee sales performance, enabling effective decision-making and strategy formulation. The dashboard leverages various data manipulation and lookup techniques to present a holistic view of our sales operations. The following guidelines outline the specific objectives and functionalities of the dashboard:

- **Data Integration**: Integrate data from orders, customers, and products tables to provide a consolidated view of sales transactions, customer information, and product details.

- **Customer Information** Lookup: Utilize XLOOKUP to efficiently retrieve the full customer name and email address from the customers table and incorporate them into the orders table, enhancing customer-centric analysis and communication.

- **Country Mapping**: Employ XLOOKUP to map the country of the customer from the customers table to the orders table, facilitating regional sales analysis and targeted marketing strategies.

- **Product Details Integration**: Utilize dynamic INDEX MATCH formulae to seamlessly integrate coffee type, roast type, size, and unit price values from the products table into the orders table. Ensure correct cell locking to automate formula application across the dataset.

- **Sales Calculation**: Calculate sales revenue by multiplying the unit price with the quantity sold, providing insights into revenue generation and product performance.

- **Standardization of Coffee Types**: Utilize multiple IF functions to standardize coffee type and roast type names, ensuring consistency in reporting and analysis.

- **Loyalty Card Status Lookup**: Utilize XLOOKUP to incorporate loyalty card status from the customers table into the orders table, enabling targeted marketing campaigns and customer loyalty analysis.

By adhering to these guidelines, the Coffee Sales Dashboard aims to empower stakeholders with actionable insights, foster informed decision-making, and drive business growth in the competitive coffee market landscape.

