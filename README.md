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

