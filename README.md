# MechaCar_Statistical_Analysis
# Overview

AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, we’ll help Jeremy and the data analytics team do the following:

* Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
* Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
* Run t-tests to determine if the manufacturing lots are statistically different from the mean population
* Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Linear Regression to Predict MPG

In the MechaCar dataset, ground_clearance and vehicle_length provided non-random amount of variance to the mpg values. In addition, there is evidence that vehicle_weight may have also provided a slight amount of variance to the mpg values, but this is not significant (if we use a significance level of 0.05).

According to the multiple linear regression model, the slope of the linear model is not considered to be zero because the p-value of the hypothesis test was 5.35e-11, which is smaller than the 0.05 significance level. 

The multiple regression model does an adequate job of predicting the mpg of MechaCar prototypes because the multiple r-squared value was 0.71. This means that roughly 71% of the time the model will predict mpg values correctly. Most likely there are other more impactful variables and factors that were not captured in the dataset that contribute to the mpg variability of the MechaCar prototypes.

![Screen Shot 2022-06-01 at 10 30 00 PM](https://user-images.githubusercontent.com/98566486/171538420-3b93b61b-1360-4802-bc0a-d077ed4567a3.png)


![Screen Shot 2022-06-01 at 10 31 01 PM](https://user-images.githubusercontent.com/98566486/171538660-ad98d9bf-3b4d-46f5-809c-b58ce5e16f9b.png)



## Summary Statistics on Suspension Coils

When looking at the entire population of the data production lots, the variance of the coils is 62.29 PSI, which is well within the MechaCar suspension coils mandate that the variance of the suspension coils cannot exceed 100 pounds per square inch (PSI).

![Screen Shot 2022-06-01 at 11 27 59 PM](https://user-images.githubusercontent.com/98566486/171546979-961bd40f-a52a-4887-9a34-4850b77c195a.png)

![Screen Shot 2022-06-01 at 11 27 44 PM](https://user-images.githubusercontent.com/98566486/171547007-54f69bc7-339f-471c-bcf0-b31de5a06eb3.png)


Lot 1 and Lot 2 are well within the 100 PSI variance requirement; with variances of 0.98 and 7.47 respectively. However, it is Lot 3 that is showing much larger variance in performance and consistency, with a variance of 170.29. It is Lot 3 that is disproportionately causing the variance at the full lot level.

## T-Tests on Suspension Coils

We conducted a t-test on the suspension coil data to determine whether there is a statistical difference between the mean of this provided sample dataset and a hypothesized, potential population dataset. Using the presumed population mean of 1500, our analysis shows:

![Screen Shot 2022-06-01 at 11 35 57 PM](https://user-images.githubusercontent.com/98566486/171547874-270b7fcc-7dbf-4cd5-bd25-dd527f88040a.png)

Assuming our significance level was the common 0.05 percent, our p-value is above our significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we would state that the two means are statistically similar.

We ran t-tests on each individual lot to further enhance our analysis:

Lot 1 actually has the true sample mean of 1500. With a p-Value of 1, we cannot reject the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500):

![Screen Shot 2022-06-01 at 11 45 58 PM](https://user-images.githubusercontent.com/98566486/171549022-0ff78c77-a757-4b94-a5cc-1211dec9e182.png)


Lot 2 has the same outcome with a sample mean of 1500.02, a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.


![Screen Shot 2022-06-01 at 11 46 07 PM](https://user-images.githubusercontent.com/98566486/171549068-1eeef769-73ae-4bfb-98fa-680b6f504a87.png)


However, Lot 3's sample mean 1496.14 is slightly lower than the popuation mean of 1500. The p-Value is 0.04, which is lower than the common significance level of 0.05. According to this lot's analysis, we can reject the null hypothesis, however, the data from this lot needs close attention. 


![Screen Shot 2022-06-01 at 11 46 21 PM](https://user-images.githubusercontent.com/98566486/171550640-0847dc7d-7d66-4b65-bae4-068a0fa108d5.png)





