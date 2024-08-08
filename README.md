# project-4-real-estate

## Real Estate Sales Price Analysis and Prediction

https://docs.google.com/presentation/d/1dwA9-JyuQVaebs8qd6LpnhV7a7wz11UBzeDLj_RRtcQ/edit?usp=sharing

https://public.tableau.com/app/profile/breanna.roybal/viz/Project4-RealEstate/PriceMedianvsBeds

https://public.tableau.com/app/profile/edward.kaczmarek/viz/shared/9W6FWHKYH

### Group 1
Vaibhav Chourasia, Eddie Kaczmarek, Koty Potts, Breanna Roybal

## Objective
The goal of our project is to analyze real estate sales data and build a machine learning model to assist investors based on various features such as the number of bedrooms, bathrooms, location, and square footage. We will also visualize the trends and patterns in the real estate market using the technologies we have learned.

## Data Description
Our data set is provided by Kaggle, and contains the following columns:

- brokered_by
    - Broker / Agency encoded
- status
    - Property of sale status
- price
    - House price
- bed
    - Number of bedrooms
- bath
    - Number of bathrooms
- acre_lot
    - Total land size / lot size in acres
- street
    - Street address encoded
- city
    - City
- state
    - State
- zip_code
    - ZIP code
- house_size
    - House size / living space in square feet
- prev_sold_date
    - Previously sold date

Data was collected from https://www.realtor.com/ - A real estate listing website operated by the News Corp subsidiary Move, Inc. and based in Santa Clara, California. It is the second most visited real estate listing website in the United States as of 2024, with over 100 million monthly active users.

## Questions to Address
- Prediction: Can we predict the sales price of a property based on its features?
- Trend Analysis: What are the trends in property sales prices over time in different locations and features?
- Correlation: How does house size correlate with actual sales prices?
- Geographical Insights: Which locations have the highest property values and sales volumes?

  # Machine Learning Analysis
  When looking at the machine learning portion of this project there can be many conclusions drawn but the main idea is that
  -analyzing property values and its features when looking at the Country level works but you can't get the accuracy to accurately predict prices
  -When building the model we need to accomodate for the social and economic side when analyzing prices
  
  #### Results of the first Regression Test
  Mean Absolute Error (MAE): 175736.6253688776
  Mean Squared Error (MSE): 107401192181.87314
  R-squared (R²): 0.48649266659831225
  Accuracy: 81.06 %.
  Mean Absolute Percentage Error (MAPE): 1893.75

  Overall we learned that by using a Random Forest Regression analysis, we were able to achieve an accuracy of 81.06%. That's really good but with a Mean Absolute Error (MAE) of 175,736. That number      sadly equates in dollars therefore we were off by $175,736 which is substantial. That is one of the main drawbacks that we learned by going at a Country-wide level.

  #### Results when going to the state of California
  Mean Absolute Error (MAE): 389305.9828040442
  Mean Squared Error (MSE): 332022036597.22687
  R-squared (R²): 0.2512681132140503
  Accuracy: 99.5 %.
  Mean Absolute Percentage Error (MAPE): 50.31

  The main reason of doing the analysis of California is because of the importance of the state in the first regression analysis. On top of that 1/5 of the data comes from California so starting from there would be the best course of action to get a higher accuracy. When looking at the results we did get a much higher accuracy but sadly the MAE is still very high with an amount of $389,304. This is most likely due to how big California is as a state and how much the price varies out there. 
  
  In order to improve this starting off with a state and then having the cities as one of the features could get us a better representation of the model for sure. On top of that once the model would be developed on a per state basis, we could potentially use it as a way to showcase estimated prices of homes in a larger/commercial scale.
