# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
The variables/coefficients that provided a non-random amount of variance are vehicle weight, spoiler angle, and AWD.

- Is the slope of the linear model considered to be zero? Why or why not?
The p-value is at 5.35e-11 which is far less than 0.05, so the slope cannot be zero.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Roughly ~71% of MPG can be predicted by this model based on the .7149 R-squared value we have, which means that we can infer there likely are other unaccounted for factors for MPG that our model doesn't account for. Which means that as a model, this prediction of MPG is ineffective.

[image]

## Summary Statistics on Suspension Coils
- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

It appears that lots 1 and 2 are within specifications, with lot 2 pushing some slightly higher variance in their data than lot 1's tight data set. Both mean and median values are at approximately 1500 for them. Lot 3 appears to be having some issues with the design specs, falling flat on the 1500 mean and median values and having a massive variance and standard deviation from the specifications dictated. Lot 2 has a large variance of 7.47, lot 3 has over 22 times that variance at 170.29 and has almost 5 times the standard deviation. Lot 3 needs to be reviewed as this poses a financial and safety risk for our customers.

[total]

[lot]

## 
