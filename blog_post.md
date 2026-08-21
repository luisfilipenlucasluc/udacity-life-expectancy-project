# What Shapes Life Expectancy in Developed Countries?

[life_expectancy_by_country.png]

Why do people live longer in some developed countries than in others? To explore this question, I analysed World Bank data for 21 countries between 2015 and 2023. The dataset combines life expectancy with GDP per capita, healthcare expenditure, internet access, unemployment, and urbanisation.

## Which factors matter most?

Healthcare expenditure and GDP per capita were the two features with the greatest influence on the model's predictions. However, these variables were also strongly related to each other, meaning that wealthier countries generally spent more on healthcare. Their influence should therefore be interpreted carefully and does not prove that either factor directly causes longer lives.

## What unexpected pattern appeared?

Eight of the ten largest annual declines in life expectancy occurred in 2020. The United States recorded the largest fall, at approximately 1.81 years, followed by Spain, Italy, and Belgium. Many countries subsequently experienced at least a partial recovery.

Another unexpected finding was the weak direct correlation between the individual predictors and life expectancy. This suggests that longevity cannot be explained by economic resources alone.

## How accurate was the model?

The Linear Regression model produced predictions that differed from actual life expectancy by approximately 0.91 years on average. Its R-squared score was 0.204, meaning that it explained 20.4% of the variation in the test data. The model therefore provides some predictive value, but important influences such as demographics, lifestyle, inequality, and healthcare quality remain outside the analysis.

## What happens in a new scenario?

For a hypothetical developed country with 95% internet usage, GDP per capita of $55,000, healthcare expenditure of $6,000 per person, 5% unemployment, and 85% urban population, the model predicted a life expectancy of **82.25 years**.

The results demonstrate both the potential and the limitations of using socioeconomic indicators to predict how long people live.
