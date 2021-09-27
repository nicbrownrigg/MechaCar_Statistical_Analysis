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

## T-Tests on Suspension Coils
Utilizing a sample population mean and a null hypothesis of "all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch", we performed T Tests on all the lots at once and the individual lots. Here's the lots as a whole:

[tTestAllLots]

Our true mean is 1498.78 like our last section. And due to our p-value being above 0.05, we cannot reject the null hypothesis.

Below are our findings for each lot:
### Lot 1
[tTestLot1]

### Lot 2
[tTestLot2]

### Lot 3
[tTestLot3]

As you can see above, all of our true means are not equal to the sample mean. After evaluating the p-values for each lot, lot 1 and lot 2 have values over 0.05 with values at 1 and .61 which means that we fail to reject the null hypothesis that they are statistically different from the sample population of 1500. However, lot 3 has a p-value of 0.04. This indicates a statistical difference from the other populations and means that lot 3, unlike the other lots, is statistically different from the sample population.

## Study Design: MechaCar vs Competition
So based on this study we've performed, in order to better tailor this to evaluate ourselves versus the competitions I would first take into account more factors to better grasp the ideal products for our customers. Since we're focusing in on fuel efficiency other than our current datapoints, I would recommend gathering metrics on: engine type, horsepower, transmission type, vehicle type, and fuel type. These are all critical factors which could impact MPG and the way our customers consider us against our competitors, so we need to consider a larger spectrum of information about our and our competition's vehicles. And by including these in our dataset along with our current datapoints, I would believe that we can narrow down the variances in our calculations. Thus moving on to the hypothesis, I would use a null hypothesis of "there is no statistically significant difference between the fuel economy of MechaCar and it's competitors." Or vis versa for an alternative hypothesis, indicating that there is a statistically significant difference in fuel economy. This can be tested by a one way ANOVA test, since we're comparing MPG across multiple groups as a whole, which is easily applicable to our null hypothesis. We would utilize sample means of MPG from MechaCar and our entire spectrum of competitors. We would run this test by using a dependant variable from our new metrics, most likely vehicle type, and MPG as an independant variable to keep ensure as much similarity of the datasets between our competitors and us as possible. 



