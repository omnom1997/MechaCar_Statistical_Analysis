# MechaCar Statistical Analysis

## Linear Regresssion to Predict MPG

We created a multiple linear regression model to see if we could predict the miles per gallon (mpg) of MechaCar prototypes based on multiple metrics collected for each vehicle such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearence. The results of our model are below:

![Linear_Regression](https://user-images.githubusercontent.com/114427019/219133999-c3f57206-4e86-477d-8219-1fdacfe6c11e.png)

As we can see, the significant variables that provided a non-random amount of variance to the mpg values were vehicle weight, spoiler angle, and AWD as these variables have "Pr(>|t|)" values for those variables are above 0.05%, our assumed significance significance level.

For the model overall, the p-value is much smaller than the assumed significance level of 0.05%. This means there there is sufficient evidence to reject our null hypothesis and that the slope of our linear model is not zero.

Although the r-squared value is high at 0.71, it's likely that our multiple linear regression mode is overfitting our data. This can be inferred from our lack of significant variables. 

## Summary Statistics on Suspension Coils

The next analysis we performed was to examine the Mean, Median, Variance, and Standard Deviation of suspension coils for MechaCar's vehicles. We performed an intial analysis of the overall summary statistics for the whole data set which is pictured below:

![Total_Summary](https://user-images.githubusercontent.com/114427019/219160047-5dba239e-2820-4378-b916-e4c4b6689cbf.png)

We then broke down the summary statistics by Manufacture's lot, and the results are included in the image below:

![Lot_Summary](https://user-images.githubusercontent.com/114427019/219160862-a46b9595-53f1-43c6-91a2-cb9bf98b5e0d.png)

The design specification for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Looking at the overall summary statistics, the variance is clearly well within the 100 pounds per square inch variance allowed by the design specifications, and thereforem meet the design specification. 

When examining each lot individually, Lot 1 and Lot 2 are within the 100 pounds per square inch variance allowed. Lot 3 is very clearly outsdie of the allocated 100 pounds per square inch of variance. Lots 1 and 2 meet the design specification, but Lot 3 do not meet the design specification.

## T-Tests on Suspension Coils

![Total_One_tail](https://user-images.githubusercontent.com/114427019/219183885-dc45f0aa-2d47-41b6-bb38-b5f53c44f186.png)

## Study Design: MechaCar vs Competition

An additional statistical study that we should perform that consumers would be interested in is city fuel efficiency. The null hypothesis could be "MechaCar vehicles are more fuel efficient than other competitors", and the alternative hypothesis could be "MechaCar vehicles are not as city fuel efficient as other competitors". We would want to use a two-sample t-test to compare MechaCar's miles per gallon against their competitors. This would be the approriate test because we are unable to compare the populations of all cars produced by MechaCar and their competitors, and two-sample t-tests compare the the distribution of means from two samples. In order to perform this statistical study, we would need to obtain a dataset with our competitors city mpg as well as collect data on MechaCar's city mpg. In the competitors' dataset, we should ensure that the data includes our competitors name, car models, and year. We should also ensure that the MechaCar data set includes year and model to help us better compare like mpg to like mpg.
