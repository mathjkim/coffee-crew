# Coffee Trading Trend Analysis

We analyze historical data on the global coffee trade from the [International Coffee Organization (ICO)](https://www.ico.org/new_historical.asp) and the [Food and Agriculture Organization (FAO) of the United Nations](https://www.fao.org). We make an interactive dashboard presenting production, consumption, exports, imports, and price for different countries and years.

<p align="center">
<img src="coffee_cover_image.jpg" width = "400" height="300" title = "Coffee Trend" />
 </p>

This project is part of The Erdös Institute's data visualization mini-course. Jimin Kim, Parham Hamidi, Anirban Sharma, and Elizabeth Campolongo collaborated to make a Tableaux story and presented it in a 2-minute video. 

## Methods
- Data Visualization: python, Tableuax
- Statistical Analysis

## Data

#### Data Collection

- Historical Data on the Global Coffee Trade https://www.ico.org/new_historical.asp 

International Coffee Organization(ICO) provides data on coffee industry over 30 years between 1990-2019. We select 9 .xlsx files: production, domestic consumption, gross opening stocks, exports, imports, re-exports, price to growers, retail price, and consumption recorded for different countries and years. 5 of them --production, domestic consumption, gross opening stocks, exports, price to growers-- includes data of the () exporting countries and 4 of them has data of of () importing countries.

- Population
- Coffee Yield per ha

#### Data Cleaning

Each excel file should be a feature in the dataframe in pandas. Our goal is to combine the tables in to one, using 'pd.melt'and 'pd.merge'. At the same time, we deal with missing values and redundant values. Also, messy string data is cleaned. 

- Structure: assign proper data type
- Quality: drop empty rows, unified format, remove unnessarily aggregated rows
- New Feature: add population and coffee yield per ha

## Analysis

1. Cross regional analysis on price paid to growers by coffee type and imports.
2. Production trend by time. 

  The production of coffee is increasing in general. It has increased more than twice compared to 30 years ago. 
72% of coffee beans are produced by Top 5 countries: Brazil, Viet Nam, Colombia, Indonesia, and Ethiopia. Among them, Brazil has consistently been at the top. The increasing trend of production by the Top 2 countries is more significant than others. There are some feature showing a linear relationship. More production leads to more exports, but over-production leads to lower prices for growers. 

3. Land efficiency of coffee producing countries.
4. Domenstic consumption vs population growth

