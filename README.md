# Brent Oil Price Event Impact Analysis
## Project Overview
This repository contains the code and documentation for Task 2 of the 10 Academy Artificial Intelligence Mastery Week 10 Challenge (19 Feb - 25 Feb 2025). The project is conducted as part of my role as a data scientist at Birhan Energies, a consultancy firm specializing in data-driven insights for the energy sector. The main goal is to analyze how significant events—such as political decisions, conflicts in oil-producing regions, global economic sanctions, and OPEC policy changes—impact Brent oil prices over the past decade.

The analysis builds on historical Brent oil price data (May 20, 1987, to September 30, 2022) and applies advanced statistical and econometric models to quantify the effects of these events. The results aim to provide actionable insights for investors, policymakers, and energy companies to navigate the volatile oil market.

## Business Objective
**The primary objective is to:**

+ Identify key events that have significantly influenced Brent oil prices over the past decade.
+ Measure the impact of these events on price changes.
+ Deliver data-driven insights to support investment strategies, policy development, and operational planning.
+ This work addresses the instability of the oil market, helping stakeholders make informed decisions, manage risks, and plan effectively.

## Dataset
**The dataset includes:**

Source: Historical Brent oil prices.
Time Period: Daily prices from May 20, 1987, to September 30, 2022.
**Fields:**
+ Date: Recorded as day-month-year (e.g., 20-May-87).
+ Price: Brent oil price in USD per barrel.
Additional data sources (e.g., economic indicators, exchange rates) may be integrated to enhance the analysis.

## Repository Structure
```/Brent-Oil-Price-Analysis
|-- /.github
|-- /.venv
|-- /.vscode
|-- /data         # Compiled list of significant events
|-- /notebooks
|   |-- Brent_Oil_Analysis_Task1.ipynb    # Data cleaning and preparation
|   |-- event_impact_analysis.ipynb                  # Exploratory Data Analysis
|   |-- indicator_analysis.ipynb # Change point detection
|   |-- price_prediction.ipynb             # Event impact modeling
|-- /scripts
|   |-- data_preprocessing.py              # Data preprocessing scripts
|   |-- data_visualizer.py                # Analysis and modeling functions
|   |-- event_change_analysis.py                   # Utility functions
|-- /src
|-- /tests
|   |-- __init__.py                    # Plots and visualizations
|   |-- test_data_preprocessor.py  # Model results and forecasts
|-- .gitignore          
|-- README.md                      # This file
|-- requirements.txt            # Python dependencies
```
## Methodology
The analysis follows a structured workflow adapted from Task 1, with a focus on applying statistical and econometric models to Brent oil price data. Below is an overview of the approach:

**1. Data Preprocessing**
+ Load and clean the Brent oil price dataset.
+ Handle missing values and anomalies.
+ Convert dates to a datetime format for time series analysis.
  
**2. Exploratory Data Analysis (EDA)**
+ Visualize price trends, volatility, and seasonality using plots (e.g., time series, rolling averages).
+ Perform statistical tests (e.g., ADF test) to assess stationarity.
  
**3. Event Identification**
+ Compile a list of significant events (e.g., geopolitical conflicts, sanctions, OPEC decisions) from the past decade.
+ Create a timeline aligning events with price data.
  
**4. Change Point Analysis**
+ Use Bayesian Change Point Detection (via PyMC3) to identify significant shifts in price behavior.
+ Apply statistical tests (e.g., Pettitt test) to confirm change points.
+ Visualize change points alongside events.
  
**5. Modeling Event Impact**
+ Event Window Analysis: Calculate price changes around event dates.
+ Regression Analysis: Use dummy variables to quantify event impacts.
+ Time Series Models: Implement ARIMA and GARCH with event exogenous variables.
+ Advanced Models: Explore VAR for multivariate analysis if additional data is included.

**6. Incorporating Additional Factors**
+ Analyze the influence of:
+ Economic Indicators: GDP growth, inflation, unemployment.
+ Exchange Rates: USD fluctuations.
+ Technological Changes: Extraction advancements, renewable energy growth.
+ Political Factors: Regulations, trade policies.
+ Integrate these variables into models where applicable.

**7. Model Validation**
+ Backtest models on historical data.
+ Perform out-of-sample testing and time series cross-validation.
+ Evaluate performance using metrics like RMSE, MAE, and R-squared.

**8. Insight Generation**
+ Summarize event impacts and rank their significance.
+ Provide price forecasts with confidence intervals.
+ Offer recommendations for stakeholders.
  
**Dependencies**
To run the code, install the required Python packages listed in requirements.txt:
```pip install -r requirements.txt```

**Key libraries include:**

pandas, numpy: Data manipulation.
matplotlib, seaborn: Visualization.
pymc3: Bayesian modeling.
statsmodels: Time series and regression analysis.
scikit-learn: Model evaluation.

**How to Run the Code**
Clone the Repository:
```git clone https://github.com/your-username/Brent-Oil-Price-Analysis.git```
cd Brent-Oil-Price-Analysis
Install Dependencies:```
pip install -r requirements.txt```

**Prepare the Data:**
Place brent_oil_prices.csv in the /data folder or load from google drive.
Run the Analysis:
Execute the Jupyter notebooks in /notebooks sequentially:

## Preliminary findings include:

Identification of key events (e.g., 2014 oil price crash due to OPEC decisions).
Quantification of price changes (e.g., percentage drops or spikes post-event).
Visualizations showing price volatility and change points aligned with events.
Detailed results are available in the /results folder and the accompanying notebooks.

## Future Work
Extend the analysis to other commodities (e.g., natural gas).
Incorporate real-time data updates for continuous monitoring.
Develop an interactive dashboard (Task 3) using Flask and React.
Contributing
Feel free to fork this repository, submit issues, or create pull requests to improve the analysis or code.

License
...

## Contact
For questions or feedback, reach out via:

GitHub: [[Jenber-Ligab](https://github.com/your-username/Brent-Oil-Price-Analysis.git)]
Email: [jenberligab@gmail.com]
