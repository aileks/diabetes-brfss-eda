# Diabetes Health Indicators EDA

Exploratory analysis of health indicators associated with diabetes status using 2015 BRFSS survey data. Focus areas include prevalence patterns, coexisting conditions, lifestyle behaviors, and socioeconomic gradients.

## Getting Started

> [!NOTE] This project is managed by [poetry](https://python-poetry.org/docs/).

Clone the repository and install dependencies:

```bash
git clone https://github.com/aileks/diabetes-brfss-eda.git
cd diabetes-brfss-eda
curl -sSL https://install.python-poetry.org | python3 -
poetry install --no-root
poetry shell
jupyter notebook diabetes_health_indicators_eda.ipynb
```

If `poetry shell` fails, enable the plugin:

```bash
poetry self add poetry-plugin-shell
```

Open `diabetes_health_indicators_eda.ipynb` and run all cells. A full PDF summary is available at: `Diabetes_Health_Analysis_Report.pdf`.

## Core Objectives

- Identify key health indicators linked with diabetes status
- Examine demographic and socioeconomic gradients
- Compare lifestyle and comorbidity patterns across groups
- Highlight potential intervention points

## Technologies Used

- Python (>= 3.11)
- pandas
- seaborn
- matplotlib
- numpy
- Jupyter
- Poetry

## Additional Documentation

- Dataset reference: [DATASET.md](./docs/DATASET.md)
- Methodology notes: [METHODOLOGY](./docs/methodology.md)

## Data Source

The data used in this analysis is based on the Behavioral Risk Factor Surveillance System (BRFSS) 2015 report, a health-related telephone survey collected annually by the CDC. The data can be found [here](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)

## References and Resources

- [CDC Behavioral Risk Factor Surveillance System (BRFSS)](https://www.cdc.gov/brfss/index.html)
- [Centers for Disease Control and Prevention - Diabetes Statistics](https://www.cdc.gov/diabetes/php/data-research/index.html)
- [National Institute of Diabetes and Digestive and Kidney Diseases (NIDDK)](https://www.niddk.nih.gov/)
