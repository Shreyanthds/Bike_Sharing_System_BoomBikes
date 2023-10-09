# Bike-Sharing System (BoomBikes) Project

## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)

## General Information

- **Project Description:** This project focuses on analyzing a bike-sharing system dataset for BoomBikes.
- **Background:** The bike-sharing system aims to optimize bike availability, marketing strategies, and pricing to meet customer demand effectively and maximize profits post-pandemic.
- **Business Problem:** Identify significant variables affecting bike demand and evaluate how well these variables explain the variation in bike demand.
- **Dataset:** The dataset contains 730 entries and 16 columns, including features like season, year, month, holiday, weather conditions, temperature, and bike demand (cnt). Data types include integers, floats, and one object column ('dteday'). No missing values were found in the dataset.

## Conclusions

- **Conclusion 1:** Key factors influencing bike demand include year, holiday, temperature, windspeed, month, weekday, and weather conditions.
- **Conclusion 2:** A multiple linear regression model (Model 8) with these significant variables provides valuable insights for predicting bike demand.
- **Conclusion 3:** The model's R-squared value of 0.843 (for training data) indicates that it explains a significant portion of the variance in bike demand.
- **Conclusion 4:** Further refinement and testing on real-world data can enhance the model's predictive accuracy, helping BoomBikes make data-driven decisions and gain a competitive edge in the bike-sharing market.

## Technologies Used

- Python - version 3.0
- pandas - version 1.0
- numpy - version 1.0
- seaborn - version 2.0
- statsmodels - version 4.0
- scikit-learn - version 0.24

## Acknowledgements

- This project was inspired by the need for BoomBikes to optimize their bike-sharing system.
- References: No specific references were used for this project.
- This project was based on data provided by BoomBikes.



## `Key Questions`

The key questions to address in this project are:
1. Identify the significant variables affecting bike demand.
2. Evaluate how well these variables explain the variation in bike demand.

## `Data Exploration`

The project began with data exploration and preprocessing. Here are the key insights:

- The dataset contains 730 entries and 16 columns, including features like season, year, month, holiday, weather conditions, temperature, and bike demand (cnt).
- Data types include integers, floats, and one object column ('dteday').
- No missing values were found in the dataset.

## `Data Visualization`

Data visualization was used to gain insights into the relationships between variables. Some key visualizations include:

- Univariate analysis: Histograms and scatterplots to examine the distribution and relationships of variables.
- Bivariate analysis: Box plots and scatterplots to analyze how categorical variables (e.g., season, month, weekday) and numerical variables (e.g., temperature) affect bike demand.
- Multivariate analysis: Pairplots and bar plots to explore interactions between multiple variables and their impact on bike demand.

## `Data Preprocessing`

Data preprocessing steps included:

1. Encoding categorical variables like season, month, weekday, and weathersit.
2. Scaling numerical variables to ensure they are on the same scale.
3. Creating dummy variables for categorical features to prepare the data for modeling.

## `Model Building`

Multiple linear regression models were built using the statsmodels library. Feature selection was performed iteratively by dropping variables with high VIF values and insignificant p-values. The final model, Model 8, included the following significant variables:

- Year (yr)
- Holiday
- Temperature (temp)
- Windspeed
- Month (except for January and February)
- Weekday (except for Monday)
- Weather conditions (Mist & Cloudy and Light Snow & Rain)

## `Model Evaluation`

The final model, Model 8, was evaluated for its statistical significance and predictive performance. Key model evaluation metrics include:

- **R-squared value:** 0.843 (indicating that 84.3% of the variance in bike demand is explained by the model).
- **AIC and BIC values:** These information criteria were used to assess the goodness of fit, with lower values indicating better fit.
- **Coefficient significance:** All selected variables were statistically significant with p-values less than 0.05.
- **Multicollinearity:** VIF values were used to check for multicollinearity, and all VIF values were below 5.

## `Conclusion`

The final multiple linear regression model provides valuable insights for BoomBikes to predict bike demand accurately.

**Key factors influencing bike demand:**

`1.year`

`2.holiday`

`3.temperature`

`4.windspeed`

`5.month`

`6.weekday`

`7.weather conditions`

This model can help BoomBikes optimize bike availability, marketing strategies, and pricing to meet customer demand effectively and maximize profits post-pandemic.

The model's `R-squared value of 0.843 for training data` and `R-squared value of 0.76 for testing data` indicates that it explains a significant portion of the variance in bike demand. Further refinement and testing on real-world data can enhance its predictive accuracy. BoomBikes can use this model as a foundation to make data-driven decisions and gain a competitive edge in the bike-sharing market.



## Contact
Created by [@shreyanthds] - feel free to contact me!
