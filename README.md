# MechaCar_Statistical_Analysis
# Overview

AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, we’ll help Jeremy and the data analytics team do the following:

* Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
* Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
* Run t-tests to determine if the manufacturing lots are statistically different from the mean population
* Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Linear Regression to Predict MPG

In the MechaCar dataset, ground_clearance and vehicle_length provided non-random amount of variance to the mpg values. In addition, there is evidence that vehicle_weight may have also provided a slight amount of variance to the mpg values, but this is not significant (if we use a significance level of 0.05). According to the multiple linear regression model, the slope of the linear model is not considered to be zero because the p-value of the hypothesis test was 5.35e-11, which is smaller than the 0.05 significance level. The multiple regression model does an adequate job of predicting the mpg of MechaCar prototypes because the multiple r-squared value was 0.71. Which means that roughly 71% of the time the model will predict mpg values correctly. Most likely there are other more impactful variables and factors that were not captured in the dataset that contribute to the mpg variability of the MechaCar prototypes.

![Screen Shot 2022-06-01 at 10 30 00 PM](https://user-images.githubusercontent.com/98566486/171538420-3b93b61b-1360-4802-bc0a-d077ed4567a3.png)


![Screen Shot 2022-06-01 at 10 31 01 PM](https://user-images.githubusercontent.com/98566486/171538660-ad98d9bf-3b4d-46f5-809c-b58ce5e16f9b.png)



## Summary Statistics on Suspension Coils

