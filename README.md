# Predicting Mobility during COVID-19
In recent years, the mobility of each country has seen drastic changes due to COVID-19. Let us predict the factors that affect mobility the most. Every country has different variables (e.g. population density, vaccination rate). How can we group countries that are similar together? By doing so, can we improve the prediction accuracy?

# Project Overview
Due to the size of the data (more than 60 columns and 160k rows), we will first use a correlation matrix to identify the variables that affect mobility the most. From observing the correlation matrix, we can identify these variables that will affect mobility the most:
1. icu_patients_per_million
2. people_vaccinated_per_hundred
3. cardiovasc_death_rate
4. aged_70_older
5. stringency index

As there is a large difference in disparity across data, K-Means clustering will be used to group similar countries together. These variables will be used in aid of clustering: 
1. gdp_per_capita
2. human_development_index
3. life_expectancy
4. population_density. 

Principal component analysis (PCA) will be applied to find the optimum amount of clusters necessary to categorise countries. After that, analysis for each of the variables identified using the correlation matrix will be analysed according to clusters to find valuable insights for each data/cluster.

Finally, the variables will be used to train multiple regression model in order to find the highest accuracy model for mobility prediction.

# Tools Used
- Principal component analysis
- K-Means Clustering
- Standard/MinMax Scaler
- Linear Regression
- Stochastic Gradient Descent
- Decision Tree Regressor

# Contribution
- Lau Yong Jie - Data preparation/cleaning, analysis, exploratory data analysis, clustering, regression
- Palaniswamy Tarun Kumar - exploratory data analysis, analysis, regression, slides & video
- Putluru Nidhi - exploratory data analysis, analysis, regression, slides & video

# References
- https://www.kaggle.com/datasets/rsrishav/world-population
- https://github.com/worldbank/covid-mobile-data
- https://seaborn.pydata.org/
