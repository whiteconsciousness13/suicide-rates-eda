### Processed Data

The processed data is stored in the `data/processed/` folder. This dataset is the result of several cleaning and transformation steps applied to the raw data to ensure it's suitable for analysis. The cleaning process includes:

1. **Dropped Irrelevant Columns**:
    - Removed columns such as `'HDI for year'` and `'suicides/100k pop'` that were deemed unnecessary for the analysis.

2. **Removed Duplicate Entries**:
    - Duplicates were removed based on the first occurrence.

3. **Handled Missing Data**:
    - Any missing data has been removed.

4. **Renamed Columns**:
    - Columns like `' gdp_for_year ($) '` were renamed for better clarity and consistency, becoming `'gdp_for_year'`.

5. **Filtered Out Irrelevant Years**:
    - Data for the year 2016 was excluded.

6. **Excluded Countries with Insufficient Data**:
    - Countries with fewer than 3 records were excluded.

7. **Cleaned Age and Sex Columns**:
    - Removed the text `" years"` from the `'age'` column.
    - Capitalized the `'sex'` column for consistency.

8. **Mapped Countries to Continents**:
    - A `'continent'` column was created by mapping countries to their respective continents. Any countries not mapped were marked as `"Unknown"` and excluded from the dataset.

9. **Converted Categorical Columns**:
    - Columns like `'sex'`, `'continent'` were converted to categorical types.
    - `'age'` and `'generation'` were converted to ordered categorical types for further analysis.
