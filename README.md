# Task 10 — Flight Operations Data Analysis

## Files
- `Flight_Operations.ipynb` — Complete Google Colab/Pandas data-analysis notebook.
- `Flight_Operations.csv` — Flight Operations dataset used in the analysis.

## Objective
Perform a complete data-analysis workflow using Pandas on the Flight Operations dataset. The notebook covers:

- Loading and understanding the dataset
- Inspecting rows, columns, data types, missing values, duplicates, and descriptive statistics
- Selecting relevant columns and rows
- Filtering records using conditions
- Sorting records
- Grouping and aggregation
- Creating transformed/derived columns
- Airline, route, weather, travel-class, booking-channel, monthly, and flight-status analysis
- Identifying patterns, operational findings, and data-quality issues
- Writing 8 key observations and a conclusion

## How to Run in Google Colab

1. Open `Flight_Operations.ipynb` in Google Colab.
2. Upload `Flight_Operations.csv` to the Colab session if it is not already available.
3. Run the notebook from top to bottom using **Runtime → Run all**.
4. Review the generated tables and analysis results.
5. Save the completed notebook if you make any additional changes.

## Repository Structure

```text
Task10/
├── Flight_Operations.ipynb
├── Flight_Operations.csv
└── README.md
```

## Main Pandas Concepts Used

`read_csv()`, `head()`, `tail()`, `shape`, `columns`, `dtypes`, `info()`, `describe()`, `isna()`, `duplicated()`, column/row selection, `loc`, `iloc`, boolean filtering, `sort_values()`, `groupby()`, `agg()`, `pd.to_datetime()`, `pd.cut()`, datetime extraction, and creation of calculated columns.

## Key Findings

- 114 of 180 flights are On Time, 59 are Delayed, and 7 are Cancelled.
- Delayed flights have lower average passenger satisfaction than on-time flights.
- Rain has the highest average delay among the weather categories.
- Vistara has the highest estimated revenue under the notebook's simple passengers × average ticket price calculation.
- Premium Economy has the highest average satisfaction among the three travel classes.
- April has the highest average delay, while March has the lowest.
- The 7 missing delay values are associated with cancelled flights.
- Some flights produce load factors above 100%, indicating a data-quality issue that should be investigated.

> **Note:** Estimated revenue is an analytical estimate, not actual accounting revenue. Load-factor anomalies are reported as data-quality findings rather than silently corrected.
