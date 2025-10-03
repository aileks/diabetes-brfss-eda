# Dataset

The dataset `diabetes_health_indicators.csv` contains survey-based health indicators derived from the Behavioral Risk Factor Surveillance System (BRFSS) of 2015.

## Variable Groups

### Health Indicators

- Diabetes_Status: No Diabetes, Prediabetes, Diabetes
- HighBP: High blood pressure status
- HighChol: High cholesterol status
- BMI: Body Mass Index
- GenHlth: Self-reported general health (Excellent to Poor)
- PhysHlth: Physical health (days not good, past 30 days)
- MentHlth: Mental health (days not good, past 30 days)

### Lifestyle Factors

- PhysActivity: Any physical activity in past 30 days
- Fruits: Fruit consumption
- Veggies: Vegetable consumption
- Smoker: Smoking status
- HvyAlcoholConsump: Heavy alcohol consumption

### Medical History

- Stroke: History of stroke
- HeartDiseaseorAttack: History of coronary event
- DiffWalk: Difficulty walking
- CholCheck: Cholesterol check in past 5 years

### Demographics

- Sex: Female or Male
- Age: Age group (18-24 to 80+)
- Education: Education level
- Income: Income bracket

### Healthcare Access

- AnyHealthcare: Has healthcare coverage
- NoDocbcCost: Skipped doctor visit due to cost

## Notes

- Some variables were recoded into descriptive labels
- Missing or ambiguous responses were retained only where analytically useful
- Numeric encodings were preserved in a parallel cleaned frame for correlation analysis
