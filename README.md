# KING COUNTY HOUSING PROJECT 
* Presented by;
    • Beatrice Kirui
    • Cliff Shitote
    • Winfred Muthoni
    • Leornard Rotich
    • Brian Kabugih

![DALL·E 2023-04-19 05.32.45](https://github.com/WinnieKabuya/dsc-phase-2-project-v2-3/blob/main/DALL%C2%B7E%202023-04-19%2005.32.45%20-%20picture%20of%20housing%20estates%20in%20the%20US.png)

## Project Overview

This project aims to use data science techniques to analyze house sales in North Western County.


The jupyter notebook for this project can be found [here.](https://github.com/Leon380/Phase-2-Project-group-2.3/blob/main/student.ipynb)

You can find the notebook [here](https://github.com/WinnieKabuya/Phase-2-Project-group-2.3/blob/main/student.ipynb)

### Business Problem

The Real Estate Agency aims to provide advice to homeowners about how home renovations might increase the estimated value of their homes, and by what amount.

### The Data

We'll be using the King County House Sales dataset.

The dataset contains:
**id** - `unique identifier for a house`

**date** - `date the house was sold`

**price** - `Sale price of the house (in dollars)`

**bedrooms** - `number of Bedrooms in a house`

**bathrooms** - `number of bathrooms in a house`

**sqft_living** - `square footage of the house`

**sqft_lot** - `square footage of the lot`

**floors** - `total floors (levels) in the house`

**waterfront** - `House which has a view to a waterfront`

**view** - `Quality of view from house`

**condition** - `How good the condition is ( Overall )`

**grade** - `overall grade given to the housing unit, based on King County grading system`

**sqft_above** - `square footage of house apart from basement`

**sqft_basement** - `square footage of the basement`

**yr_built** - `Year the house was built`


**yr_renovated** - `Year the house was renovated`

**zipcode** - `zip code in which the house is located`

**lat** - `Latitude coordinate`

**long** - `Longitude coordinate`

**sqft_living15** - `The square footage of interior housing living space for the nearest 15 neighbors`

**sqft_lot15** - `The square footage of the land lots of the nearest 15 neighbors`


## Data Cleaning and EDA

Minimal data cleaning was required, however there was a need to manage missing values,  duplicates, and outliers.
The exploratory data analysis(EDA) sought answers to the following questions:

    How does price vary with the month sold?
    How does view affect price?
    Which factors are most correlated with price?

This picture shows the home sale prices within our first time home buyers criteria by the season the house was sold. The seasons are split between spring , summer , fall  and winter. 

![seasons output.png](https://github.com/Leon380/dsc-phase-2-project-v2-3/blob/main/Image/seasons%20output.png)

We see that prices start rising from spring to summer and start dropping during summer to spring

![Viewing a house vs the price.png](https://github.com/Leon380/dsc-phase-2-project-v2-3/blob/main/Image/Viewing%20a%20house%20vs%20the%20price.png)

Houses with better views have higher prices.

Based on the questions you provided, here are some possible answers that the exploratory data analysis (EDA) may have found:

    How does price vary with the month sold?
    There is a seasonal effect on the home sale prices, with prices being higher during certain months and lower during others. For example, the analysis may have found that prices tend to be higher in the spring and summer months when the weather is better and people are more likely to be interested in buying a house. On the other hand, prices may be lower in the winter months when there are fewer buyers in the market.

    How does view affect price?
    The better the view the higher the price.

    Which factors are most correlated with price?
    Certain factors are more strongly correlated with the sale price of a house than others. For example, the size of the house (measured in square feet) may be strongly correlated with the sale price, with larger houses selling for higher prices. Other factors that may be strongly correlated with price include the location of the house (e.g., proximity to schools or public transportation), the number of bedrooms and bathrooms, and the condition of the house.

  ## Modeling and Predictions
  
  ![Residual QQ plot output.png](https://github.com/Leon380/dsc-phase-2-project-v2-3/blob/main/Image/Residual%20QQ%20plot%20output.png)
  
  Since almost all of the data points fall along a straight line in this QQ-plot, we can consider the normality assumption satisfied.
  
  ![Residual scatterplot output.png](https://github.com/Leon380/dsc-phase-2-project-v2-3/blob/main/Image/Residual%20scatterplot%20output.png)
  
  The scatterplot appears to show a roughly symmetrical and consistent spread of the residuals around the lowess regression line, suggesting that the homoscedasticity
  assumption is met for the Model.
  

  **Regression results**
  
  Model 1
  
  The model explains about 49% of the variance in price.
  The p_values are zero therefore less than the threshold value of 0.05 therefore the model is statistically significant
  
  Model 2
  
  The model explains about 58.1% of the variance in price.
  The p_values are zero therefore less than the threshold value of 0.05 therefore the model is statistically significant
  
  Final- model:
  
  The model explains about 63% of the variance in price which is an improvement from the previous model.

  ## Conclusion

  The creation of these models will enable the Real Estate Agency to provide precise valuations of residential properties to their customers. Moreover, by comprehending the aspects that significantly affect the selling price, the agency can suggest homeowners on how to boost their home's worth via enhancements or modifications. Overall, this venture can furnish meaningful understandings about the determinants that sway the sale price of a house in King County, benefiting both the Real Estate Agency and their clientele.
