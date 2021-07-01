# Phase Two Project Repo
<img src="../images/KingCounty.jpeg">

# Overview
This project dives into a slice of the King County, Washington real estate market. We seek to use linear regression to build a predictive model that will best predict sale price of a house for our clients. We looked at a variety of ranging from location, phyiscal atributes of the home, residential building grades, proximity to Whole Foods, and median household income. We found many features that contributed to our model producing more accurate predictions. We found the X and Y had the largest impact on our model. Additionally by manipulating these features, they also were very impactful... Next steps for us would be to gather some additional census data to give us more continuous data for income levels in each neighborhood. 
# Business Problem
We have been hired by a Seattle based Real Estate Brokerage to build a model that will help them accurately predict home prices so they can better serve their clients when helping them buy or sell their home. We would like to investigate how various internal features of a home effect price as well as external features of the larger neighborhood.
# Data
We used 3 data sources for this project.
1. Housing data on about 21,000 homes in King County that was given to us
2. Whole Foods location data found on Kaggle
3. Median income by zip code obtained from  IPUMS' (Integrated Public Use Microdata Series) National Historic Geographic Information System
# Methods
We prepared our data by cleaning and combining into one dataframe to begin to model. We began with the basic process of testing out features to see which were most effecting our model. We proceeded with feature engineering and scaling to arrive at our final model which utilized 15 features, one hot encoder, the linear regression model from the sklearn package, train-test split, and the standard scaler.
# Results
* Train Test Split Error Scores: 
Test Root Mean Squared Error: 149120.457
Train Root Mean Squared Error: 147543.401
* Cross Validation Score: 0.717
* Quantile Test:
Most error is between 854 thousand and 2 million. The error in all other bins is around 30 thousand dollars down to 5.5 thousand dollars for one bin.
# Conclusion and Next Steps
In conclusion, we ended up using a more basic regression method than we anticipated. The two most impactful features on our model were two that we engineered. The highest being the square root of sq_ft_above with a coefficient of nearly 200,000 and the second highest being the interaction between square foot living, grade, and nearest Whole Foods being -150,000. This interaction is negative because the smaller the distance to Whole Foods, the greater the price of the home. Initial next steps for us would be to take more census data into account around income and schools, accessibility to municipal services, and additional features of the home such as size of driveway, type of heating, or existence of porch. Finally, we would like to create a model with price per square foot as the target as that would leave much less room for error and could help us better hone in on the best model possible.
project-folder
    |
    README.md
    data-folder
    images-folder
    notebooks-folder
          |
          report.ipynb
          exploratory-folder
                  |
                  CeCe-notebooks-folder
                  kyle-notebooks-folder 
                  Warren-notebooks-folder 