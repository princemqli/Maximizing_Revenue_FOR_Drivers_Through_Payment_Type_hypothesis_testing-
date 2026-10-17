Maximizing Revenue for Taxi Drivers Through Payment Type Analysis
Project Overview
This project analyzes NYC Yellow Taxi trip data to investigate whether the average fare amount differs between passengers who pay by card and those who pay by cash. Python, data visualization, and hypothesis testing are used to explore payment behavior and identify useful business insights.
Business Problem
Taxi drivers and operators want to understand whether payment method is associated with differences in trip fare amounts. This analysis compares card and cash transactions to test whether the observed difference in average fares is statistically significant.
Project Objectives
- Compare average fare amounts for card and cash payments.
- Explore trip distance, trip duration, and passenger-count patterns.
- Visualize payment preferences and fare distributions.
- Use a statistical hypothesis test to assess the difference in average fares.
- Translate the findings into practical, data-informed business recommendations.
Dataset
The notebook uses NYC Yellow Taxi trip records for January 2020 (yellow_tripdata_2020-01.csv).
The analysis focuses on fields such as:
- Pickup and drop-off datetime
- Passenger count
- Trip distance
- Payment type
- Fare amount
Dataset note: The CSV is loaded from a Google Colab path in the notebook. Upload the dataset to your runtime or update the file path before running the notebook. Follow the dataset provider's terms when sharing data.
Tools and Technologies
- Python
- Jupyter Notebook / Google Colab
- Pandas — data cleaning and analysis
- Matplotlib and Seaborn — visualizations
- SciPy — statistical hypothesis testing
- Statsmodels — statistical analysis support
Workflow
1. Load the taxi trip dataset.
2. Inspect the data structure and data types.
3. Convert pickup and drop-off timestamps and calculate trip duration.
4. Select relevant columns for the analysis.
5. Filter for card and cash payments and reasonable passenger counts.
6. Clean invalid values and inspect fare outliers.
7. Explore fare amounts, trip distances, payment preferences, and passenger counts using charts and summary statistics.
8. Compare card and cash fare amounts using an independent two-sample Welch's t-test.
9. Interpret the p-value at a 5% significance level.
Hypothesis Testing
Null hypothesis (H₀): The mean fare amount is the same for card and cash trips.
Alternative hypothesis (H₁): The mean fare amount differs between card and cash trips.
- Significance level: 0.05
- Test: Independent two-sample Welch's t-test (equal_var=False)
- Decision rule: If the p-value is below 0.05, reject the null hypothesis.
The notebook reports a statistically significant difference in average fare amounts between card and cash trips. This indicates an association in the analyzed data; it does not establish that the payment method itself causes higher fares.
Key Findings
- The notebook compares average fare amounts and trip distances by payment type.
- Visualizations show the distributions of fares, trip distances, payment preferences, and passenger counts.
- The hypothesis test reports a p-value below the 5% significance level, so the null hypothesis is rejected.
- The result suggests that average fare amounts differ between card and cash trips in the cleaned sample.
Business interpretation: Card payments may be associated with higher average fares in this dataset. Drivers and operators could make card payments convenient for passengers, while avoiding claims that changing payment method alone will increase revenue. Trip distance, trip duration, location, time, tips, and other factors may also influence the observed differences.
How to Run
1. Download or clone this repository.
2. Install the required libraries:pip install pandas matplotlib seaborn scipy statsmodels jupyter
3. Place yellow_tripdata_2020-01.csv in the location expected by the notebook, or update the CSV path in the first data-loading cell.
4. Open the notebook in Jupyter or Google Colab.
5. Run the cells in order.
Repository Contents
- Maximizing_Revenue_FOR_Drivers_Through_Payment_Type_hypothesis_testing.ipynb — notebook containing the analysis, visualizations, and hypothesis test.
- yellow_tripdata_2020-01.csv — input dataset, if you choose to include it and are permitted to redistribute it.
Limitations
- The analysis identifies differences between groups but does not prove causation.
- Fare amounts can be affected by trip distance, duration, location, time, surcharges, and other factors.
- Cleaning rules and outlier removal can affect the results.
- The findings apply to the selected dataset and period; they may not represent all taxi trips or current behavior.
Conclusion
This project demonstrates a complete exploratory data analysis and hypothesis-testing workflow using Python. It compares card and cash taxi trips, visualizes passenger and trip patterns, and evaluates whether average fares differ statistically. The results can inform further investigation into payment behavior and taxi revenue.
Skills demonstrated: Data Cleaning • Exploratory Data Analysis (EDA) • Data Visualization • Hypothesis Testing • Statistical Analysis • Python
