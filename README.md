# Diabetes Health Indicators - Exploratory Data Analysis

An exploratory data analysis project examining health indicators and their relationship with diabetes prevalence using data from the Behavioral Risk Factor Surveillance System (BRFSS).

## Overview

This project analyzes a comprehensive dataset of health indicators to understand factors associated with diabetes status (no diabetes, prediabetes, and diabetes). The analysis explores demographic factors, lifestyle behaviors, comorbidities, and socioeconomic indicators to identify patterns and risk factors for diabetes.

## Objectives

The analysis aims to:

1. Identify which health indicators are most strongly associated with diabetes status
2. Examine how demographic factors correlate with diabetes risk
3. Explore relationships between modifiable risk factors and diabetes
4. Suggest potential intervention points for diabetes prevention

## Dataset

The dataset (`diabetes_health_indicators.csv`) contains health survey data with the following features:

### Health Indicators

- **Diabetes_Status**: Diabetes diagnosis (No Diabetes, Prediabetes, Diabetes)
- **HighBP**: High blood pressure status
- **HighChol**: High cholesterol status
- **BMI**: Body Mass Index
- **GenHlth**: Self-reported general health (Excellent to Poor)
- **PhysHlth**: Physical health (days not good in past 30 days)
- **MentHlth**: Mental health (days not good in past 30 days)

### Lifestyle Factors

- **PhysActivity**: Physical activity in past 30 days
- **Fruits**: Fruit consumption
- **Veggies**: Vegetable consumption
- **Smoker**: Smoking status
- **HvyAlcoholConsump**: Heavy alcohol consumption

### Medical History

- **Stroke**: History of stroke
- **HeartDiseaseorAttack**: History of heart disease or attack
- **DiffWalk**: Difficulty walking
- **CholCheck**: Cholesterol check in past 5 years

### Demographics

- **Sex**: Gender (Male/Female)
- **Age**: Age group (18-24 to 80+)
- **Education**: Education level
- **Income**: Annual household income

### Healthcare Access

- **AnyHealthcare**: Healthcare coverage status
- **NoDocbcCost**: Could not see doctor due to cost

## Key Findings

### 1. **Age and Diabetes**

- Diabetes prevalence increases dramatically after age 45
- Rates more than double in elderly populations (over 20% in 65+ age groups)
- Strong age-related progression suggests need for age-appropriate screening

### 2. **BMI Distribution**

- Clear relationship between higher BMI and diabetes
- Median BMI: ~30 (diabetes), ~29 (prediabetes), ~25 (no diabetes)
- Higher concentrations of diabetic individuals in overweight/obese ranges

### 3. **Comorbidities**

- Diabetic individuals show significantly higher rates of:
  - High blood pressure (73% vs 38%)
  - High cholesterol (67% vs 35%)
  - Heart disease (22% vs 7%)
- Prediabetes represents an intermediate risk state

### 4. **Lifestyle Factors**

- Lower physical activity rates among diabetic individuals (63% vs 78%)
- Fruit and vegetable consumption lower in diabetic group
- Lifestyle modifications show potential for prevention and management

### 5. **Socioeconomic Gradients**

- Inverse relationship between education level and diabetes prevalence
- Higher income associated with lower diabetes rates (25% lowest vs 8% highest income)
- Social determinants significantly impact diabetes risk

### 6. **General Health Perception**

- Diabetic individuals report significantly lower general health
- Most common ratings: "Good" or "Fair" vs "Very Good" in non-diabetic group
- Diabetes significantly impacts quality of life

## Technologies Used

- **Python 3.11+**
- **pandas**: Data manipulation and analysis
- **seaborn**: Statistical data visualization
- **matplotlib**: Plotting and visualizations
- **numpy**: Numerical operations
- **Jupyter Notebook**: Interactive analysis environment

## Prerequisites

This project uses Poetry for dependency management. Make sure you have Python 3.11 or higher installed.

## Getting Started

### Installation

1. Clone the repository:

```bash
git clone https://github.com/aileks/diabetes-brfss-eda.git
cd diabetes-brfss-eda
```

2. Install Poetry (if not already installed):

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

3. Install dependencies:

```bash
poetry install
```

4. Activate the virtual environment:

```bash
poetry shell
```

### Running the Analysis

1. Launch Jupyter Notebook:

```bash
jupyter notebook
```

2. Open `diabetes_health_indicators_eda.ipynb` in your browser

3. Run all cells to reproduce the analysis and visualizations

Alternatively, view the pre-generated outputs:

- `Diabetes_Health_Analysis_Report.html` - HTML version of the notebook
- `Diabetes_Health_Analysis_Report.pdf` - PDF version of the notebook

## Analysis Structure

The notebook is organized into the following sections:

1. **Data Loading and Preparation**

   - Import libraries and load dataset
   - Check for missing values
   - Data type conversions

2. **Data Cleaning and Transformation**

   - Map numerical codes to descriptive labels
   - Create clean dataset for visualization

3. **Problem Definition**

   - Define research questions and objectives

4. **Descriptive Statistics**

   - Dataset overview
   - Distribution analysis
   - Cross-tabulations

5. **Visualizations**

   - Diabetes status distributions
   - BMI analysis
   - Age-related patterns
   - Comorbidity comparisons
   - Lifestyle factor analysis
   - Correlation matrices
   - Socioeconomic analysis
   - Risk factor combinations

6. **Conclusions**
   - Summary of findings
   - Implications for prevention and treatment

## Visualizations

The analysis includes comprehensive visualizations:

- Distribution plots for diabetes status
- Box plots and violin plots for BMI analysis
- Stacked bar charts for age-related patterns
- Heatmaps for correlation analysis
- Comparative bar charts for health conditions and lifestyle factors
- Scatter plots for multi-factor relationships

## Key Insights for Healthcare

This analysis highlights several actionable insights:

- **Modifiable risk factors**: Physical activity, diet, and weight management show clear associations with diabetes risk
- **Target populations**: Elderly individuals (65+) and those with high BMI warrant increased screening
- **Comprehensive care**: Strong comorbidity patterns suggest need for integrated cardiovascular and metabolic care
- **Social interventions**: Education and income disparities point to opportunities for public health policy interventions

## Data Source

The data used in this analysis is based on the Behavioral Risk Factor Surveillance System (BRFSS), a health-related telephone survey collected annually by the CDC.

## References

- CDC Behavioral Risk Factor Surveillance System (BRFSS)
- Centers for Disease Control and Prevention - Diabetes Statistics
- National Institute of Diabetes and Digestive and Kidney Diseases (NIDDK)

---

> [!NOTE]
> This is an educational project for exploratory data analysis. The findings should not be used as medical advice. Always consult healthcare professionals for medical decisions.
