# Global Petroleum Market Analysis

## Overview
A Python exploratory data analysis project integrating two country-level datasets covering petroleum consumption, reported fuel prices, GDP per capita, and fuel-affordability indicators.

The supplied files each contain 181 records. After validating country keys, the one-to-one merge matched all 181 country records across both files.

## Questions explored
- Which countries have the highest reported daily oil consumption?
- Which countries have the highest reported fuel prices per liter?
- How are GDP per capita and reported fuel prices associated?
- How do median reported fuel prices differ by continent?

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, PyCountry, CountryInfo, Jupyter Notebook.

## Initial data-derived observations
- The United States has the largest reported daily oil consumption in the supplied data: 19,687,287 barrels per day.
- The median reported fuel price is approximately USD 1.40 per liter across 181 records.
- The Spearman rank correlation between GDP per capita and reported fuel price is approximately 0.429 for records with both values.

These are descriptive results from the supplied files, not independently verified current market statistics. The source publication dates, original URLs, and variable definitions should be documented before treating them as externally validated findings. The source data includes potentially unusual observations (for example, very high reported prices) that should be checked against the original source.

## Data quality and limitations
- The two files were loaded with `cp1252` encoding.
- All 181 country keys matched in a one-to-one merge.
- Geographic enrichment uses ISO alpha-3 codes plus a documented fallback mapping for dataset-specific country/territory labels. The latest run resolved all 181 records with no missing ISO-3 codes or continent assignments. Broad Americas labels were normalized to North America or South America for consistent continent-level summaries. Review the fallback mapping if the source dataset changes.
- Fuel price and GDP associations do not imply causation.
- The data's reference year and source provenance have not been established from the CSV files alone.
- Confirm that source-data redistribution is permitted before publishing the CSVs publicly.


## Author
Emmanuel Odili

Data Analytics | Business Intelligence | Python | SQL | Power BI

[LinkedIn Profile](https://www.linkedin.com/in/odiliemmanuel)
