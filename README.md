# Shopping Trends Analysis (notebook)

This repository contains a Jupyter Notebook `project.ipynb` that performs exploratory data analysis on `shopping_trends.csv` using pandas and matplotlib.

## What the notebook does

- Loads `shopping_trends.csv` into a pandas DataFrame.
- Shows basic inspection: `head()`, `info()`, `describe()`, `shape`.
- Checks for missing values and duplicates.
- Plots distributions and summaries for columns including `Age`, `Gender`, `Season`, `Category`, `Color`, `Payment Method`, `Purchase Amount (USD)`, and `Review Rating`.
- Uses group-by and aggregation to compute sums/means for fields like `Purchase Amount (USD)` by `Season`, `Payment Method`, and `Size`.
- Builds pie charts, bar plots, histograms, boxplots, and scatter plots to visualize relationships.

## Dependencies

- Python 3.8+ (or 3.x)
- pandas
- matplotlib
- numpy

You can install the dependencies with:

pip install pandas matplotlib numpy

## How to run

1. Open `project.ipynb` in Jupyter Notebook or VS Code and run the cells sequentially.
2. Ensure `shopping_trends.csv` is in the same directory as the notebook.

## Observations & Notes (based on reading the notebook)

- The notebook performs EDA and visualizations but does not modify or save cleaned data.
- Visualizations include: histograms for `Age` and `Purchase Amount (USD)`, bar charts for category counts, pie charts for payment method and season totals, boxplots comparing purchase amounts across frequency groups, and scatter plots comparing previous purchases to review rating.
- There are group-by summaries for `Season`, `Payment Method`, `Size`, and `Color` (mean review rating, sums of purchase amounts, etc.).
- The notebook currently assumes column names match exactly; no explicit error handling is included for missing columns.
- Some cells create plots without clearing figures between them; when run in sequence this is fine, but when re-running single cells in a long session, call `plt.clf()` if needed.

## Suggested next steps

- Add a small data-cleaning section to handle missing values and standardize column names.
- Add comments or markdown cells explaining key findings (e.g., which season has highest spending, which payment methods are most popular).
- Save key summary tables to CSV for downstream use.
- Improve plots with labels, percentages on pie charts, and color palettes for readability.
- Add a requirements.txt or environment.yml for reproducibility.

## Contact

If you'd like, I can help: add cleaning steps, create clearer visualization code (with seaborn), or produce a short report summarizing the top insights with code cells that produce the exact numbers and plots referenced.
