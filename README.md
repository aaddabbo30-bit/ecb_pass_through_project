# ECB Policy Rate Pass-Through (MRO → Bank Lending Rates)

This project analyses how the **ECB main refinancing operations (MRO)** rate transmits into **bank lending rates** for households and firms in the euro area.

## Data
- **FM (Key interest rates)**: Main refinancing operations – minimum bid/fixed rate (daily, Euro area).
- **MIR (MFI interest rate statistics, monthly, new business)**:
  - Households – consumption loans
  - Households – house purchase loans
  - Non-financial corporations – loans over €1M, 1–5 years

Data are publicly available from the [ECB Data Portal](https://data.ecb.europa.eu).

## Method
- Converted daily MRO series to monthly frequency.
- Merged with monthly MIR lending rates.
- Visualised time-series comparisons (MRO vs loans).
- Calculated cross-correlations at lags 0–12 months.
- Estimated OLS regressions with MRO lags (1–3 months).

## Results
The analysis confirms a strong pass-through from the ECB policy rate to household and corporate lending rates, with different lags across loan categories.

## Technologies used
- Python 3
- pandas, matplotlib, statsmodels
- Jupyter Notebook

## Skills Demonstrated
- Data management (cleaning, merging, resampling)
- Statistical analysis (cross-correlation, OLS with lags)
- Visualisation of policy-relevant results
