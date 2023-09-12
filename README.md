# Factors-influencing-US-Home-prices
Predicting US Home Prices: Analyzing key factors impacting home prices in the US over 36 years (1987-2023) using data science techniques.
Data Science Project: Factors Affecting US Home Prices

Introduction: 
This data science project aims to comprehensively analyse the key factors influencing home prices in the United States over the last 36 years. We will delve into multiple datasets related to housing market indicators, such as population, housing supply, GDP, mortgage rates, and employment rates, all sourced from [FRED (Federal Reserve Economic Data)]( https://fred.stlouisfed.org/ ). The project's objective is to identify the primary drivers behind fluctuations in housing prices and construct predictive models to gain insights into and forecast future trends.
Data Preparation and Loading: 
In this section, we meticulously prepare and load the requisite datasets for analysis:
1. House Price Index (CSUSHPISA): This dataset serves as the cornerstone, containing historical data on the US Housing Price Index (CSUSHPISA), our target variable.
2. Population: It encompasses data on the US population over time, a fundamental demographic indicator.
3. Housing Supply: This dataset provides valuable insights into housing supply metrics.
4. GDP: Contains Gross Domestic Product (GDP) data for the US economy, an indicator of economic health.
5. Mortgage Rates: This dataset includes mortgage rate information, a critical variable impacting the housing market.
6. Employment Rate: It furnishes data on the employment rate in the United States, a significant economic indicator.




We ensure that all datasets have a consistent date format and have been adjusted for seasonality, with the date range spanning from January 1987 to May 2023, covering the last 36 years.



Data Exploration:
Data Overview:
Our exploration begins with an in-depth examination of the structure and summary statistics of our merged dataset. The combined dataset comprises 437 entries and 7 columns, including 'DATE,' 'CSUSHPISA,' 'Population,' 'Housing_supply,' 'GDP,' 'MORTGAGE30US,' and 'Employment_rate.' We provide key statistics, such as means, standard deviations, minimum, and maximum values, for each column.
Outlier Detection:
To guarantee data quality, we meticulously identify potential outliers in the 'CSUSHPISA' column. By calculating the Interquartile Range (IQR) and defining lower and upper bounds, we ensure the reliability of our data.

Data Visualization:
We harness the power of visualizations to extract insights from the data:
Scatter Plot:
We craft a scatter plot to visually uncover the relationship between 'Population' and 'CSUSHPISA.' The scatter plot reveals a non-linear correlation, implying that as population increases, 'CSUSHPISA' tends to rise, but not at a constant rate.
Correlation Matrix Heatmap:
A heatmap vividly displays the correlation matrix, allowing us to grasp the interplay between variables. Notably, 'CSUSHPISA' exhibits a robust positive correlation with 'Population,' 'MORTGAGE30US,' and 'Employment_rate.'
Distribution Plots:
We construct distribution plots for key variables ('CSUSHPISA,' 'Population,' 'Housing_supply,' and 'GDP') to identify patterns and understand their distributions.
Time Series Plot:
Visualizing the time series data of 'CSUSHPISA' over time unveils an upward trend. This suggests that the CSUSHPISA index has been steadily ascending since January 1987, covering the last 36 years, with hints of seasonality and cyclicity.




Data Modelling:
Data Splitting:
Our data is judiciously partitioned into training and testing sets, with 80% dedicated to training and 20% for testing. This segmentation allows us to effectively train and evaluate our machine learning models.
Model Selection:
We embark on an exploration of various regression models to predict 'CSUSHPISA':
Linear Regression
Lasso Regression
Ridge Regression
Random Forest Regressor
Gradient Boosting Regressor
For each model, we assess performance using metrics like Mean Squared Error (MSE) and R-squared.

Regularized Models:
We delve deeper into model refinement by implementing regularization techniques for two models:
Random Forest Regressor (Regularized)
Gradient Boosting Regressor (Regularized)
These models undergo optimization with regularization to enhance predictive accuracy.

Results and Conclusion:
The project culminates in a thorough analysis of model performance, including MSE and R-squared values. Our regularized models, specifically the Random Forest Regressor and Gradient Boosting Regressor, demonstrate exceptional performance with minimal MSE values (close to 2.5) and R-squared values nearing 0.9995.
In conclusion, this project underscores the significance of population, housing supply, GDP, mortgage rates, and employment rates, all sourced from FRED, in influencing US home prices over the last 36 years. The predictive models developed offer actionable insights for comprehending and forecasting trends in the US housing market, with practical applications in pricing strategies and real estate investment decisions.


