
# Maximizing Revenue for Taxi Drivers Through Payment Type Analysis

## Project Overview
This project analyzes NYC Yellow Taxi trip data to understand the relationship between payment type and fare amount. Python, data visualization, and hypothesis testing are used to compare card and cash transactions.

## Objectives
- Compare average fare amounts for card and cash payments.
- Analyze trip distance and passenger count.
- Visualize payment preferences and fare distributions.
- Perform hypothesis testing to check whether average fares differ significantly.
- Generate useful business insights from taxi trip data.

## Dataset
The project uses NYC Yellow Taxi trip data for January 2020.

**Dataset:** `yellow_tripdata_2020-01.csv`

Important features include:
- Pickup and drop-off datetime
- Passenger count
- Trip distance
- Payment type
- Fare amount

## Tools and Technologies
- Python
- Jupyter Notebook / Google Colab
- Pandas
- Matplotlib
- Seaborn
- SciPy
- Statsmodels

## Project Workflow
1. Load the dataset.
2. Explore the data structure and data types.
3. Clean the data and handle invalid values.
4. Calculate trip duration.
5. Analyze card and cash transactions.
6. Visualize fare amounts and trip distances.
7. Perform statistical hypothesis testing.
8. Interpret the results and identify business insights.

## Hypothesis Testing

**Null Hypothesis (H₀):** The average fare amount is equal for card and cash transactions.

**Alternative Hypothesis (H₁):** The average fare amount differs between card and cash transactions.

- Significance Level: 0.05
- Statistical Test: Welch's Two-Sample t-test

**Decision Rule:** If the p-value is less than 0.05, reject the null hypothesis.

## Key Findings
- The project compares average fares for card and cash transactions.
- Visualizations help identify patterns in fares, trip distances, and payment preferences.
- The notebook reports a statistically significant difference in average fare amounts between the two payment groups.
- The results indicate an association between payment type and fare amount, but do not prove that payment type causes higher fares.

## Business Recommendations
- Make card payments convenient for passengers.
- Analyze trip distance, duration, and other factors alongside payment type.
- Use data-driven insights to improve taxi business decisions.
- Avoid assuming that payment method alone will increase revenue.

## How to Run the Project

### 1. Install the Required Libraries

```bash
pip install pandas matplotlib seaborn scipy statsmodels jupyter
```

### 2. Prepare the Dataset
Download or obtain `yellow_tripdata_2020-01.csv` and update the dataset path in the notebook if necessary.

### 3. Open the Notebook
Open the `.ipynb` file in Jupyter Notebook or Google Colab.

### 4. Run the Analysis
Execute the notebook cells in order to reproduce the data analysis, visualizations, and hypothesis test.

## Repository Contents
- `Maximizing_Revenue_FOR_Drivers_Through_Payment_Type_hypothesis_testing.ipynb` — Jupyter Notebook containing the analysis.
- `yellow_tripdata_2020-01.csv` — Dataset used for the project, if included.

## Limitations
- The analysis identifies associations, not causation.
- Fare amounts may depend on distance, duration, location, time, tips, and other factors.
- The results apply to the selected dataset and period.
- Data cleaning and outlier treatment can affect the findings.

## Conclusion
This project demonstrates data cleaning, exploratory data analysis, data visualization, and statistical hypothesis testing using Python. It explores differences in taxi fares by payment type and provides insights that can support further business analysis.

---

**Skills:** Python | Data Cleaning | EDA | Data Visualization | Hypothesis Testing | Statistical Analysis

