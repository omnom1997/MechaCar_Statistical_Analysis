# MechaCar Statistical Analysis

## Linear Regresssion to Predict MPG

We created a multiple linear regression model to see if we could predict the miles per gallon (mpg) of MechaCar prototypes based on multiple metrics collected for each vehicle such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearence. The results of our model are below:

![Linear_Regression](https://user-images.githubusercontent.com/114427019/219133999-c3f57206-4e86-477d-8219-1fdacfe6c11e.png)

As we can see, the significant variables that provided a non-random amount of variance to the mpg values were vehicle weight, spoiler angle, and AWD as these variables have "Pr(>|t|)" values for those variables are above 0.05%, our assumed significance significance level.

For the model overall, the p-value is much smaller than the assumed significance level of 0.05%. This means there there is sufficient evidence to reject our null hypothesis and that the slope of our linear model is not zero.

Although the r-squared value is high at 0.71, it's likely that our multiple linear regression mode is overfitting our data. This can be inferred from our lack of significant variables. 
