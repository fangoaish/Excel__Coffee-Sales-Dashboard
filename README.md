# Coffee Sales Dashboard

## Project Overview

The goal of this project is to develop an interactive dashboard using Microsoft Excel. This dashboard will enable users to quickly identify trends in coffee bean sales and make comparisons across different bean types and countries.


<img width="1353" alt="Overview of Coffee Sales Dashboard" src="https://github.com/fangoaish/Excel__Coffee-Sales-Dashboard/assets/51399519/f53cc2bf-279b-4256-b2b9-658a1012cabd">


## Scope
This project involves end-to-end data analysis in Excel, from data gathering to data cleaning and transformation, all the way to creating meaningful visualizations in the form of a dynamic, interactive dashboard.

## Project Steps
1. Data Gathering
2. Data Preparation Using Advanced Formulas and Functions
3. Exploratory Data Analysis
4. Data Visualizations And Dashboard Build Using **Pivot Tables**, **Pivot Charts**, **Timeline** and **Slicers**

## Data Sources
- Coffee Bean Sales
  - coffeeOrderData.csv 

## Data Gathering
The data source is a fictitious coffee bean sales dataset provided by Mo Chen. Link [HERE](https://github.com/mochen862/excel-project-coffee-sales). 

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
Gain comprehensive insights into global workout demand, popular fitness keywords, regional interest splits, and preferred workout types in the Philippines and Singapore. These insights will inform strategic decisions regarding digital product offerings and market positioning for the fitness studio in Singapore.

- Evaluate the global demand for workouts from mid-March 2018 to mid-March 2023.
- Investigate the top three fitness keywords that garnered the highest interest during different time intervals.
- Assess the distribution of interest across these keywords in the Philippines and its neighboring countries, including those in the Middle East.
- Determine the most popular workout types in the Philippines and Singapore.

   


### **Findings**
Over the past 5 years, the keyword _**'workout'**_ has played the dominant role compared to others in Singapore; whereas, _**'zumba'**_ is the most popular search, followed by the second highest one - _**'workout'**_ in the Philippines.

![Yotuube sports keyword searches in the singapore over the past 5 years](https://github.com/fangoaish/Python__Digital-Fitness-Product-Strategy-for-Singaporean-Market-Positioning/assets/51399519/e9f4014b-373e-4da2-87fb-2f2597f0d188)

![Yotuube sports keyword searches in the philippines over the past 5 years](https://github.com/fangoaish/Python__Digital-Fitness-Product-Strategy-for-Singaporean-Market-Positioning/assets/51399519/8153ce46-456e-472f-9f24-d90f218e1e78)


### **Recommendations**
- Customize content and campaigns based on local keyword trends.
- Develop products aligned with specific market interests.
- Enhance competitiveness by refining offerings based on keyword insights.


## Limitations
- Quality of Datasets: The reliability of the findings and the effectiveness of proposed recommendations heavily rely on the quality and completeness of the datasets provided. Incomplete or inaccurate data could lead to biased analysis and misleading conclusions.
- Dependency on External Tools: The analysis involves reliance on external tools such as Google Trends and Youtube Keyword Searches. Any limitations or inaccuracies in these tools could affect the accuracy of the analysis results.



