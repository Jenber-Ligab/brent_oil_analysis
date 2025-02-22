# Brent Oil Price Analysis - Task 1

This project implements Task 1 of the 10 Academy Week 10 Challenge (19 Feb - 25 Feb 2025), focusing on defining the data analysis workflow and understanding the model and data for Brent oil prices, as tasked by Birhan Energies.

## Structure
- `data/`: Contains `brent_oil_prices.csv` (assumed input with 'Date' and 'Price' columns).
- `scripts/`: Python modules for the analysis.
  - `__init__.py`: Makes scripts a package.
  - `preprocessing.py`: Cleans and prepares data.
  - `notebooks/`: Jupyter Notebook directory.
  - `Brent_Oil_Analysis_Task1.ipynb`: Invokes scripts and displays results.
- `plots/`: Directory for saved plots (optional if save_plots=True).
- `requirements.txt`: List of dependencies.

## Business Objective
Analyze how significant events (political decisions, conflicts, sanctions, OPEC policies) affect Brent oil prices to provide insights for investors, policymakers, and energy companies at Birhan Energies.

## Requirements
- Python 3.8+
- pandas, numpy, matplotlib, jupyter

## Usage
1. Place `brent_oil_prices.csv` in `data/` (format: 'Date' as 'dd-mmm-yy', 'Price' in USD/barrel).
2. Install dependencies: `pip install -r requirements.txt`.
3. Run the notebook:
   - `cd brent_oil_analysis/`
   - `jupyter notebook notebooks/Brent_Oil_Analysis_Task1.ipynb`
   - Execute all cells.

## Outputs
- **Notebook Inline:**
  - Sample raw and processed data.
  - Summary statistics.
  - Visualizations: Price trend, volatility, price distribution.
  - Model definitions, data generation details, assumptions, and communication plans.
- **Plots Directory (optional):** Saved visualizations if `save_plots=True`.