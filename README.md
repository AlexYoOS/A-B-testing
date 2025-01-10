# Analyze A/B Test Results

This project involves analyzing the results of an A/B test run by an e-commerce website. The goal is to determine whether the new landing page leads to more conversions compared to the old landing page.

## Project Structure

- `Analyze_ab_test_results_notebook.ipynb`: Jupyter notebook containing the analysis of the A/B test results.
- `ab_data.csv`: Dataset containing the A/B test results.
- `countries.csv`: Dataset containing the country information of users.

## Analysis Steps

1. **Data Wrangling**:
   - Load and inspect the datasets.
   - Clean the data by removing rows with mismatched group and landing page assignments.
   - Check for missing values and duplicates.

2. **Exploratory Data Analysis (EDA)**:
   - Calculate the number of unique users.
   - Determine the proportion of users who converted.
   - Analyze the distribution of conversions across different groups.

3. **A/B Test Analysis**:
   - Perform hypothesis testing to compare the conversion rates between the control and treatment groups.
   - Use bootstrapping to simulate the sampling distribution of the difference in conversion rates.
   - Calculate the p-value and interpret the results.

4. **Regression Analysis**:
   - Perform logistic regression to analyze the impact of the landing page on conversion rates.
   - Include additional factors such as country to see if they influence conversion rates.
   - Test for interaction effects between the landing page and country.

## Key Findings

- The analysis did not find significant evidence to suggest that the new landing page leads to more conversions compared to the old landing page.
- The logistic regression analysis also did not show significant effects of the landing page or country on conversion rates.

## Conclusion

Based on the analysis, it is recommended not to switch to the new landing page as there is no significant improvement in conversion rates. Further analysis with additional factors and a larger sample size may be needed to make a more informed decision.

## How to Run the Notebook

1. Ensure you have Jupyter Notebook installed.
2. Place the `ab_data.csv` and `countries.csv` files in the same directory as the notebook.
3. Open the `Analyze_ab_test_results_notebook.ipynb` file in Jupyter Notebook.
4. Run the cells sequentially to reproduce the analysis.

## Dependencies

- Python 3.x
- pandas
- numpy
- matplotlib
- statsmodels

Install the required packages using:
```bash
pip install pandas numpy matplotlib statsmodels
```

## Author

This project was completed as part of the Udacity Data Analyst Nanodegree program.
