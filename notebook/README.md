# Notebooks Folder Description

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

- Key findings and insights from the data analysis are summarized.
- The notebook provides a complete end-to-end analysis pipeline from data cleaning to visualization.

## File

- **Notebook File**: [Suicide Rate Analysis Notebook](notebook/rtp.ipynb)

This notebook contains all the steps of data cleaning, transformation, and analysis for the suicide rate dataset.
