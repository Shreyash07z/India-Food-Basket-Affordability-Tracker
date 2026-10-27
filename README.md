## Indian Mandi Vegetable Price Analysis

A pandas-based analysis of daily mandi prices for selected vegetables across Indian markets, exploring seasonal trends, price volatility, and regional differences.

> **Note:** Mandi prices are wholesale market prices. They do not represent the retail prices consumers pay in shops.

## Project question

How do modal prices for selected vegetables change across Indian mandi markets over time, and which months tend to have the highest prices?

## Project goals

- Prepare and clean daily market price data using pandas.
- Compare modal prices for selected vegetables across markets.
- Summarize price patterns by month to explore seasonality.
- Identify periods and commodities with larger price changes or volatility.
- Document data cleaning choices and limitations so the analysis is reproducible.

## Data source

The project uses the Government of India's **Current Daily Price of Various Commodities from Various Markets (Mandi)** dataset, published on the [Open Government Data Platform India](https://www.data.gov.in/resource/current-daily-price-various-commodities-various-markets-mandi).

Download the CSV from the dataset page and place it in the project as described in the notebook. The available date range and fields may change as the source is updated. Record the download date and the exact file used when you begin the analysis.

## Analysis plan

1. Inspect the data structure, column types, missing values, and duplicate records.
2. Standardize column names and parse the arrival date.
3. Check price fields for invalid or implausible values.
4. Select a consistent set of vegetables and markets for comparison.
5. Aggregate modal prices by month and compare trends across markets.
6. Present findings with charts and explain the limits of the data.

The dataset commonly includes fields such as state, district, market, commodity, variety, arrival date, and minimum, maximum, and modal prices. Confirm the actual column names in the downloaded file before running analysis; names can differ by file version.

## Repository structure

```text
.
├── data/                 # Local data files (not committed by default)
├── notebooks/            # Jupyter notebooks for exploration and analysis
├── README.md
└── requirements.txt      # Add dependencies used by the project
```

Adjust this structure to match the files in your repository.

## Getting started

1. Clone this repository.
2. Download the CSV from the official dataset page and place it in the expected local data folder.
3. Install the Python packages listed in `requirements.txt`.
4. Open the notebook in `notebooks/` and run the cells in order.

If you have not created a `requirements.txt` yet, add the packages you actually use. For the current pandas-based analysis, that will at least include `pandas`; add plotting or notebook packages if your project uses them.

## Planned outputs

- Monthly modal-price trends for selected vegetables.
- Comparisons of price levels across selected markets.
- A summary of seasonal patterns and notable price movements.

This section should be updated with specific findings after the analysis is complete.

## Limitations

- Mandi prices are wholesale prices and should not be described as retail affordability or household grocery costs.
- Markets may report different varieties or grades, which can make direct comparisons imperfect.
- Reporting coverage, missing values, and the available date range may vary over time.
- Seasonal patterns describe associations in the observed data; they do not establish what caused a price change.

## Project status

In progress.

## License and data use

The dataset is provided by the Government of India through the Open Government Data Platform. Review the dataset page and its applicable terms before redistributing the raw data. This repository's code and documentation are separate from the source dataset.
