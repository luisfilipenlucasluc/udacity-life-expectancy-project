# Predicting Life Expectancy Using World Development Indicators

## Project Motivation

Life expectancy is an important indicator of a country's health and socioeconomic development.

This project uses data from the World Bank's World Development Indicators to analyse how economic, healthcare, employment, urbanisation, and digital-access factors relate to life expectancy.

The main objective is to train a machine learning model capable of predicting life expectancy at birth.

## Business Questions

1. Which socioeconomic indicators have the strongest relationship with life expectancy?
2. What unusual or unexpected patterns can be identified across countries and years?
3. How accurately can a machine learning model predict life expectancy?
4. What life expectancy would the model predict for a hypothetical country with a specific socioeconomic profile?

## Dataset

The dataset was obtained from the World Bank's World Development Indicators database.

It contains 189 observations covering 21 countries between 2015 and 2023. Each observation represents one country in one year.

The variables used in the analysis are:

- Life expectancy at birth
- GDP per capita
- Health expenditure per capita
- Unemployment rate
- Urban population
- Internet usage
- Year

Life expectancy is the target variable. The remaining numeric variables are used as predictive features.

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Repository Files

- `udacity-life-expectancy-project.ipynb`: Jupyter Notebook containing the data preparation, exploratory analysis, modelling, evaluation, visualisations, feature importance analysis, and predictive scenario.
- `README.md`: Project description, motivation, methodology, file information, results, and acknowledgments.
- `blog_post.md`: Non-technical blog post presenting the main findings of the analysis.
- `life_expectancy_by_country.png`: Visualisation of life expectancy trends across the 21 selected countries between 2015 and 2023.
- `world_bank_data/`: World Development Indicators dataset and supporting metadata files obtained from the World Bank DataBank.

## Methodology

The project follows the CRISP-DM process:

1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Modeling
5. Evaluation
6. Communication of Results

The original data was reshaped so that each row represented one country in one year. The transformed dataset contained no missing values or duplicate rows.

A Linear Regression model was trained using 80% of the observations and evaluated on the remaining 20%.

## Summary of Results

The Linear Regression model achieved the following results:

- Mean Absolute Error: 0.91 years
- Root Mean Squared Error: 1.09 years
- R-squared score: 0.204

The model's predictions differed from the actual life expectancy values by approximately 0.91 years on average. The model explained approximately 20.4% of the variation in life expectancy within the test data.

GDP per capita and health expenditure were the most influential features in the model's predictions. However, these variables were strongly correlated, so their individual importance should be interpreted carefully.

The analysis also identified a notable temporal pattern: eight of the ten largest annual declines in life expectancy occurred in 2020. The United States recorded the largest decline, followed by Spain, Italy, and Belgium.

For the hypothetical scenario, the model predicted a life expectancy of 82.25 years.

## Blog Post

The public blog post presenting the findings in non-technical language will be linked here after publication.

## Acknowledgments

The data used in this project was obtained from the World Bank's World Development Indicators database.

The analysis was completed as part of the Udacity Data Scientist Nanodegree project. AI tools were used to support code review, troubleshooting, and language refinement. All analysis, implementation decisions, and final validation were completed by the project author.