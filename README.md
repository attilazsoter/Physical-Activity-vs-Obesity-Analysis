# Physical Activity and Obesity Data Analysis

This project analyzes the relationship between physical activity and obesity prevalence across the United States using publicly available survey data. It explores whether different forms of exercise — such as aerobic activity and weight training — have measurable effects on obesity rates, and evaluates the role of activity intensity, frequency, and duration.

The work combines exploratory data analysis, statistical testing, and visualization to assess exercise effectiveness and provide insights relevant for both individuals and public health policymakers.

## Objectives

Test the null hypothesis that physical activity has no significant effect on obesity.

Compare the effectiveness of aerobic activity vs. weight/muscle training.

Identify which exercise factors (frequency, intensity, duration, type) most strongly correlate with obesity prevalence.

Provide evidence-based insights that could support health policy initiatives and obesity-prevention strategies.

## Data Source

Dataset: Nutrition, Physical Activity, and Obesity - Behavioral Risk Factor Surveillance System (BRFSS)
Published by: U.S. Department of Health & Human Services

Dataset (CSV format): https://healthdata.gov/dataset/Nutrition-Physical-Activity-and-Obesity-Behavioral/fhdq-98vk/about_data

Data Dictionary (key metadata): https://chronicdata.cdc.gov/Nutrition-Physical-Activity-and-Obesity/Nutrition-Physical-Activity-and-Obesity-Behavioral/hn4x-zwk7/about_data

Coverage: 2011–2023
Size: ~104,000 rows, 33 attributes

Key attributes include:

Demographics: Age, Gender, Race/Ethnicity, Income, Education

Measures: Obesity, overweight, physical activity intensity/frequency

Geography: U.S. states + territories

## Methodology
### 1. Data Cleaning & Preparation

Removed unnecessary columns and standardized variable names (e.g., YearStart → Year, LocationDesc → State).

Converted categorical variables to string types.

Pivoted survey questions into structured columns.

Addressed missing values; excluded insufficient samples (e.g., Virgin Islands, Puerto Rico).

### 2. Exploratory Data Analysis (EDA)

Examined completeness of state-year responses.

Analyzed obesity vs. physical activity trends across time and geography.

Created aggregated datasets at the state-year level.

### 3. Statistical Analysis

Ran correlation analysis between obesity and multiple activity measures.

Calculated Pearson correlation coefficients and p-values to validate significance.

Identified the strongest predictors of obesity reduction.

### 4. Visualization

Scatterplots comparing obesity with aerobic and muscle training activities.

Correlation heatmaps across states and exercise measures to highlight key patterns.

## Key Findings

Strong negative correlations exist between aerobic activity and obesity rates.

The most effective combination against obesity was found to be:

At least 150 minutes of moderate/75 minutes of vigorous aerobic activity per week, plus at least 2 days of weight training.
This showed the highest correlation with reduced obesity (-0.867).

States with higher aerobic participation consistently reported lower obesity rates.

Muscle training alone showed weaker impact, but when combined with aerobic activity, it significantly enhanced outcomes.

Increasing aerobic duration beyond 300 minutes weekly appeared to yield diminishing returns.

## Tools & Libraries

Python (Jupyter Notebook):

pandas – data wrangling

matplotlib, seaborn – visualization

scipy.stats – correlation and hypothesis testing

## Conclusion

The analysis confirms that physical activity plays a critical role in reducing obesity, with aerobic activity being the strongest individual predictor. Combining aerobic and muscle-strengthening exercises produced the most significant effects.

These findings support the importance of encouraging regular physical activity through public health campaigns and policy interventions to combat rising obesity rates.
