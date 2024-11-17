This folder contains the Jupyter Notebook used for the **suicide rate analysis** project. The notebook is structured to perform the following tasks:

## Data Import and Cleaning

- The dataset is imported from a CSV file and cleaned by removing unnecessary columns, handling missing values, and transforming column names.
- Duplicate rows are dropped, and rows with missing values are removed.
- The dataset is filtered to exclude entries for the year 2016 and countries with fewer than three entries.

## Data Transformation

- The **age** column is cleaned by removing the unit text ("years").
- The **sex** column is capitalized to ensure consistent formatting.
- The **continent** column is added by mapping countries to their respective continents.
- **Nominal columns** like `country`, `sex`, and `continent` are converted to categorical types, while `age` and `generation` are set as ordered categorical variables.

## Analysis and Visualizations

- The cleaned dataset is analyzed to explore trends and patterns in suicide rates across different demographics like age, gender, and continent.
- Various visualizations are created to represent the insights.

## Conclusion

This analysis of global suicide rates across various demographics (gender, age, country, and continent) reveals significant trends that can be pivotal in understanding mental health issues globally. Key findings include:

- Peak suicide rate was 15.7 deaths per 100k in 1995
- Decreased to 10.8 per 100k in 2015
- Europe has the highest rate
- Trends for Africa are inaccurate due to poor quality data
- Both male & female suicide rates peaked in 1995
- Globally, suicide rate increases with age
- Lithuania has the highest rate
- I analyzed average GDP per capita (wealth) versus overall suicide rates for each country. To understand the potential link between economic well-being and suicide rates, I calculated the mean GDP per capita for each country across all years with available data. This provides a single value representing a country's average wealth. I then compared this value to the country's overall suicide rate across the same period.
- Hence, GDP (per capita) explains very little of the variance in suicide rate overall. There is a weak but significant positive linear relationship - richer countries are associated with higher rates of suicide, but this is a weak relationship which can be seen from graph abov

## File

- **Notebook File**: [Suicide Rate Analysis Notebook](/notebook/rtp.ipynb)

This notebook contains all the steps of data cleaning, transformation, and analysis for the suicide rate dataset.
