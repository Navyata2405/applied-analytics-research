# Social Assistance Classification

## Project Overview

This project explores the use of machine learning to identify households that may require social assistance based on their income and living conditions.

The objective is to develop a classification model that can help identify population groups in need of financial support, assist cities and municipalities with resource allocation, and better understand socioeconomic patterns associated with social assistance requirements.

## Research Objectives

- Develop a classification model to identify households requiring social assistance.
- Explore socioeconomic characteristics and patterns within the dataset.
- Investigate the relationship between household income, living conditions, and social assistance.
- Evaluate and optimize the performance of a Decision Tree classification model.

## Dataset

**Source:** Urban Mobility Survey, Brazil (2016), obtained through Kaggle.

The dataset contains 19,252 complete and valid household responses, representing information on 61,358 residents across the Federal District of Brazil.

The original survey was designed to investigate urban mobility patterns and socioeconomic characteristics of the population.

## Methodology

The project follows the following analytical approach:

1. **Data Cleaning and Preprocessing:** Handling missing values, checking duplicates, and preparing relevant variables for analysis.
2. **Exploratory Data Analysis:** Examining household characteristics, income distributions, and relationships between variables through statistical summaries and visualizations.
3. **Correlation Analysis:** Investigating relationships between explanatory variables.
4. **Model Development:** Implementing a Decision Tree classification model to predict social assistance requirements.
5. **Model Optimization:** Testing different maximum tree depths to evaluate model performance and potential overfitting.

## Model

The primary algorithm used in this project is the **Decision Tree Classifier**, implemented using Python's Scikit-learn library.

The dataset is divided into training (70%) and testing (30%) subsets.

Different maximum tree depths are evaluated to compare training and testing accuracy and investigate model generalization.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Repository Structure

```text
social-assistance-classification/
│
├── README.md
├── data/
│   └── Household.csv
│
└── social_assistance_classification.ipynb
```

## Limitations and Future Considerations

The model is limited by the variables available in the original dataset. Additional socioeconomic characteristics, including education, outstanding loans, age, and years in the workforce, could provide further insight into household eligibility for social assistance.

Further model evaluation using additional classification metrics would also help assess the model's ability to identify households requiring assistance.

## References

- Urban Mobility Survey, Brazil (2016), dataset obtained through Kaggle.
