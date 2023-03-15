# MechaCar_Statistical_Analysis

## Overview
* AutosRUs' newest prototype, the MechaCar, is suffering from production troubless that are blocking the manufacturing team's progress. The data analytics team need to review the production data f tor insights that may help the manufacturing team.

* The analysis include:
    * Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
    * Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.
    * Run t-tests to determine if the manufacturing lots are statistically different from the mean population.
    * Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.


## Linear Regression to Predict MPG

![image](https://user-images.githubusercontent.com/114631804/224904926-0b0a1d12-77ee-44a1-8c74-d341ec00231b.png)

* The variables in our dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance.The linear repression model run on these variables agaisnt figures for MPG, resulted in p-values of 2.6x10-12 and 5.21x10-8. 

* As the p-value is 5.35x10-11, which is lower than the level of significance, the null hypothesis should be rejected. There for the slope of the linear model cannot be considered to be zero.

* This model does predict the MPG of the MechaCar prototype somewhat effectively since the r-squared value is 0.7149, indicates that the model is 71% accurate.

## Summary Statistics on Suspension Coils

![image](https://user-images.githubusercontent.com/114631804/225208570-3171ab08-9a67-4d09-a78e-9a4a9659106c.png)

![image](https://user-images.githubusercontent.com/114631804/225208665-04c3e507-bf2d-4a7a-9fe3-5148a27c2499.png)

* As shown above, the overall variance is under 100 psi and meet specifications. However, the variance for Lot 3 is at 170.29 which is well above the acceptable threshold, which might indicate some potential problem with this lot.

## T-Tests on Suspension Coils

### T-test for all lots
* According to the suspension Coils Cumulative T-test, the suspension coils across all manufacturing lots show that they are not statistically different from the population mean, approximately 1500 psi. The p-value is 0.06028, not low enough to reject null hypothesis.

![image](https://user-images.githubusercontent.com/114631804/225216738-e162c0c4-3f11-4f4a-b6c4-771d5f5826d1.png)


* The result of the T-test for the suspension coils for Lot 1 show no statistical difference to population mean and the p-value is 1, not low enough to reject the null hypothesis.

![image](https://user-images.githubusercontent.com/114631804/225218493-2e04561d-abe9-469d-b25c-44ffd02a06c7.png)


* The result of the T-test for the suspension coils for Lot 2 show no statistical difference to population mean and the p-value is 0.6072, not low enough to reject the null hypothesis.

![image](https://user-images.githubusercontent.com/114631804/225218418-90ba52e2-0d80-46ec-8db3-a21cd60a9631.png)


* The result of the T-test for the suspensio coils for Lot 3 show a slight different to population mean. The p-value is 0.04168, which is lower than the common 0.05. Therefore, the null hypothesis can be rejected, which determined that this lot might has potential problem and need further evaluation.

![image](https://user-images.githubusercontent.com/114631804/225219595-968c4dbc-7e1c-4df2-a784-0ee1898554e0.png)

## Study Design: MechaCar vs Competition 

There are many factors that customer would consider before purchase a car, for example, price, fuel efficiency, safety rating, maintenance cost, etc. However, with the price of gas increase and booming of hybrid and electric vehicles, consumers really consider fuel efficiency is one the of the big factors.

### Metric to test

We should research and evaluate MechaCar's fuel efficiency, especially within city roads and highways.

### Null and Alternative Hypothesis

Null: MechaCar's prototype consumes the same amount of fuel compare to competitor's vehicle.

Alternative: MechaCar's prtotype does NOT consume the same amount of fuel compare to competitor vehicle (could be more or less).

### Statistical Test to Use

The best statistical test to use for this analysis would be two-sample T-test.

### What data is needed

The analysis will required fuel consumption data for both MechaCar's prototype and competitor vehicles.
