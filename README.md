# Weather EDA & Hypothesis Testing Project

This project focuses on analyzing weather data from Los Angeles across the years 2022 and 2023. It combines exploratory data analysis (EDA) with non-parametric hypothesis testing to uncover patterns and statistical relationships among key weather variables.

## Objective

The goal of this project is to use real-world weather data to:
- Understand seasonal trends and variation in temperature, humidity, visibility, and cloud cover
- Explore relationships between weather variables
- Statistically test hypotheses about those relationships using appropriate non-parametric methods

## Dataset

The dataset includes daily weather readings for Los Angeles and contains variables such as:
- `datetime`: Date of observation
- `temp`: Actual temperature
- `feelslike`: Perceived temperature
- `humidity`: Humidity level
- `cloudcover`: Percentage of sky covered by clouds
- `visibility`: Visibility score
- `conditions`: Categorical label of weather conditions (e.g., Clear, Rain, Cloudy)

## Tools Used

- Python (Pandas, NumPy)
- Visualization: Seaborn, Matplotlib
- Statistical Testing: Scipy, Pingouin
- Jupyter Notebook (via VS Code)

## Exploratory Data Analysis

The project explores:
- Monthly average trends in temperature and humidity
- Comparison of actual vs. feels-like temperature
- Visibility variation based on cloud cover and weather condition
- Distributions of key numerical features using line plots, boxen plots, violin plots, KDE plots, and scatter plots

## Hypothesis Testing

The following hypotheses were tested:

1. **Is there a difference between actual and feels-like temperature?**
   - Test used: Wilcoxon Signed-Rank Test
   - Result: Failed to reject the null hypothesis

2. **Do weather conditions affect visibility?**
   - Test used: Kruskal–Wallis H-test
   - Result: Rejected the null hypothesis

3. **Is cloud cover correlated with visibility?**
   - Test used: Spearman correlation
   - Result: Rejected the null hypothesis (negative correlation)

## Key Insights

- Temperature and humidity follow clear seasonal trends.
- In most cases, actual and feels-like temperatures are statistically similar.
- Higher cloud cover is associated with lower visibility.
- Weather conditions significantly impact visibility patterns.

## Conclusion

This project demonstrates how visual and statistical analysis can work together to draw meaningful insights from real-world data. Through a combination of EDA and hypothesis testing, we validated several intuitive relationships and uncovered subtle patterns across time.

## How to Use

Clone the repository, open the Jupyter notebook in `notebooks/`, and run the cells to explore the data and replicate the analysis.

```bash
git clone https://github.com/suzaladhikari/la-weather-statistical-analysis.git
cd la-weather-statistical-analysis
jupyter notebook
