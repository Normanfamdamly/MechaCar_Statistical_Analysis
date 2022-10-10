# MechaCar_Statistical_Analysis - Module 15 Challenge

## Linear Regression to Predict MPG
---
The R Script was applied to the MechaCar_mpg.csv to get the following coefficients.

![length_weight_spoiler_clear_mpg.png](https://github.com/Normanfamdamly/MechaCar_Statistical_Analysis/blob/main/images/length_weight_spoiler_clear_mpg.png)

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

- There is a 95% confidence level as predetermined, which infers the p-value should be compared to an         alpha of .05 to have statistical significance.
  - AWD: .19>=.05 not statistically significant, random amount of variance.
  - Ground Clearance: 0> .05 statistically significant, non-random amount of variance.
  - MPG: 0<.05 statistically significant, non-random amount of variance.
  - Spoiler Angle: .31 > .05 not statistically significant, random amount of variance.
  - Vehicle Length: 0 < .05, statistically significant, non-random amount of variance.
  - Vehicle Weight: .08 > .05 not statistically significant, random amount of variance.
  
![Coefficients.png](https://github.com/Normanfamdamly/MechaCar_Statistical_Analysis/blob/main/images/Coefficients.png)

2.  Is the slope of the linear model considered to be zero? Why or why not?

- As see above the coefficients are all in scientific notation. But once they are converted, they are shown to be close to zero or non-zero.  
    - AWD: - 3.4.11
    - Ground Clearance: 3.546
    - MPG: -.01
    - Spoiler Angle: .069
    - Vehicle Length: 6.267
    - Vehicle Weight: 6.267
  Multiple Linear Regression =  -.01(MPG)+6.267(VL)+.069(SA)+3.546(GC)+-3.411(AWD)
  
  ![lm.png](https://github.com/Normanfamdamly/MechaCar_Statistical_Analysis/blob/main/images/length_weight_spoiler_clear_mpg.png)

3.  Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

-  The R-square measures the proportion of variation in the dependent variable. Our R-squared is .7149 which is a strong correlation for the dataset we are reviewing for MechaCar. While not the only variable for consideration is doesn’t provide a positive attribute to consider.

## Summary Statistics on Suspension Coils
---
The Mean for the manufacturing lots is 1498.78 and the Median is 1500 with a Variance of 62.29356 and a Standard Deviation of 7.892627.

![Total_Summary.png](https://github.com/Normanfamdamly/MechaCar_Statistical_Analysis/blob/main/images/Total_Summary.png)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

![Lot_Summary.png](https://github.com/Normanfamdamly/MechaCar_Statistical_Analysis/blob/main/images/Lot_Summary.png)

Over all Variance is 62 which is less than 100 which is within the required design specifications of under 100 PSI.  But when you review the data by Lots you see a large difference between the lots.  Lots 1 and 2 have Variances of 1 and 7 respectively, but Lot 3 is 170 which is greater than the 100 specifications.

## T-Tests on Suspension Coils
---
![Suspension_Coil_PSI.png](https://github.com/Normanfamdamly/MechaCar_Statistical_Analysis/blob/main/images/Suspension_Coil_PSI.png)

- All Manufacturing Lots as seen above have a MEAN of 1498.78 which we saw in the summary statistics above and a p-value of 1 which we cannot reject the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).

![Lot1_TTest.png](https://github.com/Normanfamdamly/MechaCar_Statistical_Analysis/blob/main/images/Lot1_TTest.png)

- Lot 1 has a p-value that is .000000000001568 which is less than .05(alpha) which is statistically significant  and indicates strong evidence against the null hypotheses as these is less than a 5% probability the null is correct. Therefore, we accept the alternative hypothesis.

![Lot2_TTest.png](https://github.com/Normanfamdamly/MechaCar_Statistical_Analysis/blob/main/images/Lot2_TTest.png)

- Lot 2 has a p-value of .5911 > .05 which means Lot 2 is not statically significant from the normal distribution and normality can be assumed. The mean falls with the 95% confidence interval.

![Lot3_TTest.png](https://github.com/Normanfamdamly/MechaCar_Statistical_Analysis/blob/main/images/Lot3_TTest.png)

- Lot 3 is .1589 which is > .05 and is not statically significant and indicates strong evidence for a null hypothesis and a rejection of the alternative hypothesis.
Over all Variance is 62 which is less than 100 which is within the required design specifications of under 100 PSI.  But when you review the data by Lots you see a large difference between the lots.  Lots 1 and 2 have Variances of 1 and 7 respectively, but Lot 3 is 170 which is greater than the 100 specifications.



## Study Design: MechaCar vs Competition
---
