## Linear Regression to Predict MPG

<img width="620" alt="Screen Shot 2022-06-17 at 11 06 53 AM" src="https://user-images.githubusercontent.com/100390727/174335714-6fb07967-f00a-4e26-999e-1a1cd26326bc.png">


According to our summary output, the two variables that provided a non-random variance to the dataset's MPG variables are the vehicle length and ground clearance. These two variables significantly impact the miles per gallon for our MechaCar prototypes. When looking at the P-values produced from our code output, we see that the other variables (vehicle weight, spoiler angle, and AWD) have random variance.

The slope of this linear model is not zero, and this is evident by looking at the P-value of our model which is 5.35e-11 and comparing it to 0.05, which is the assumed significance level. The P-value is much smaller than 0.05, which tells us that the slope is not zero.

This linear model definitely predicts the MPG of the MechaCar prototypes effectively. When looking at the r-squared value, we can see that it is 0.7149. This signifies that about 71% of all of the predictions about MPG can be determined by this model. This percentage is relatively high, telling us that this is an effective approach that we've taken.

## Summary Statistics on Suspension Coils

<img width="619" alt="Screen Shot 2022-06-17 at 11 16 29 AM" src="https://user-images.githubusercontent.com/100390727/174337167-8b744847-8294-4300-a8b2-596f0a6a5def.png">

<img width="619" alt="Screen Shot 2022-06-17 at 11 17 04 AM" src="https://user-images.githubusercontent.com/100390727/174337236-c593fd63-a3b1-4449-a7bc-143790976501.png">

**The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?**

Looking at the variance of the coils in the total_summary dataframe above, we see that the value is 62.29356. This does not exceed the 100 pound limit, which is good. The issue comes with the variance observed in the other dataframe (lot_summary). The variance for Lot1 is approximately 0.98 while the variance for Lot2 is around 7.46. These two lots are well below the 100 pound limit, however we can see that the variance for Lot3 is about 170.29. Lot3 is the issue here, because it has too high of a variance.

## T-Tests on Suspension Coils

<img width="487" alt="Screen Shot 2022-06-17 at 2 34 47 PM" src="https://user-images.githubusercontent.com/100390727/174390606-5b3500e4-40a9-4831-ab5b-de052d13fe9c.png">

The first T-test outcome printed to our console shows the mean of the sample as 1498.78. The p-value is 0.6028, which is a higher value than 0.05 which is the common significance level. 

<img width="465" alt="Screen Shot 2022-06-17 at 2 39 11 PM" src="https://user-images.githubusercontent.com/100390727/174391106-0bf61588-14ce-4802-818a-f0587384c833.png">


When looking at the 3 lots individually, we see that lot1 has a mean of 1500, lot2 has a mean of 1500.2 and lot3 has a mean of 1496.14. 
lot1 has a p-value of 1, while the p-value of lot2 is 0.6072 and the p-value of lot3 is 0.04168. It should be noted that lot3's p-value is lower than 0.05 which is the common significance level. This means that we should reject the null hypothesis stating that this sample mean and the presumed population mean are not statistically different. Special attention and further analysis should be given to lot3, as there may be suspension coils that don't meet the desired criteria.

## Study Design: MechaCar vs Competition

There are potential statistical studies that could be implemented to quantify how the MechaCar performs against any competition. First, we would have to decide which MechaCar model stands out and is able to be a good comparison with the competitor. The competitor's cars must be examined to find the most similar model worthy of being compared to the chosen MechaCar.

Metrics that could be tested are:
1. Engine: whether it be a hybrid, electric, etc.
2. MPG: how well each car performs when looking at the miles per gallon.
3. Price: how much is each car? How much does the average owner have to spend per year on each car?
4. Resale Value: How much are people buying the used cars for?

*Null Hypothesis*
MechaCar has a fair price considering all of it's factors.

*Alternative Hypothesis*
Considering all that it has to offer, MechaCar has an unfair price.

## Statistical Tests

In order to run the hypothesis, there would need to be some statistical tests done. I think the best test considering our hypothesis would be a multiple linear regression. A multiple linear regression model is defined as a regression model that estimates the relationship between a quantitative dependent variable and two or more dependent variables using a straight line. This would be a very effective way at testing our hypothesis.

