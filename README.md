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

