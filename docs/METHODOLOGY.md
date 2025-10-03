# Methodology

## Objectives

1. Identify health indicators most associated with diabetes status
2. Examine demographic patterns and socioeconomic gradients
3. Assess relationships between modifiable behaviors and diabetes
4. Flag intervention points for prevention and early management

## Processing Steps

1. Load raw CSV and standardize data types
2. Rename `Diabetes_012` to `Diabetes_Status`
3. Map coded categorical values to descriptive labels
4. Create cleaned copy (`df_clean`) for presentation and a numeric frame for correlation
5. Engineer composite metrics (e.g., risk score from blood pressure, cholesterol, BMI tier)

## Analysis Components

- Distribution profiling (status, BMI, age)
- Cross-tabulations (age × status, education × status, income × status)
- Condition prevalence comparisons (hypertension, cholesterol, heart disease, stroke)
- Lifestyle behavior contrasts (activity, diet proxies, alcohol)
- Correlation matrix of numeric health indicators
- Risk score stratification
- Multivariate visualizations (BMI by activity, BMI and age vs status)

## Visualization Approach

- Seaborn for statistical plots (box, violin, bar, scatter, heatmap)
- Consistent palette for categorical comparability
- Percentage normalization for stacked and grouped views

## Assumptions

- Self-reported measures introduce bias but remain directionally informative
- Education and income act as proxies for broader socioeconomic determinants
- Physical activity variable is treated as a binary exposure indicator

## Limitations

- Cross-sectional survey; no causal inference
- Self-report recall and social desirability bias
- Limited dietary granularity (fruit and vegetable simplifications)
- No direct measures of blood glucose or A1C

## Reproducibility

Run the notebook `diabetes_health_indicators_eda.ipynb` top to bottom after installing dependencies. All figures are generated programmatically without manual editing.
