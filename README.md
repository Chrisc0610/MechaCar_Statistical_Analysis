# MechaCar_Statistical_Analysis  

## Linear Regression to Predict MPG

**Statistical Summary:** 
- ![linear_regression.PNG](/Resources/Images/linear_regression.PNG)

From the above output we can see that:

 - The **vehicle length**, and **ground clearance** are statistically likely to provide non-random amounts of variance to the model. 
That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely,
the **vehicle weight**, **spoiler angle**, and **All Wheel Drive** (AWD) have p-Values that indicate a random amount of variance with the dataset.  

 - The p-Value for this model, ```p-Value: 5.35e-11```, is much smaller than the assumed significance level of 0.05%. 
	This indicates there is sufficient evidence to **reject our null hypothesis**, which further indcates that the slope of this linear model is **not zero**.


 -  This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. 
	Relatively speaking, his multiple regression model **does predict mpg of MechaCar prototypes effectively**. 




# Deliverable 2:  

## Summary Statistics on Suspension Coils
- ![summary_statistics.PNG](/Resources/Images/summary_statistics.PNG)


 - When looking at the entire population of the production lot, the variance of the coils is 62.29 PSI, which is well within the 100 PSI variance requirement.  

 -  Lot 1 and Lot 2 are well within the 100 PSI variance requirement; with variances of 0.98 and 7.47.  
	It is Lot 3 that is showing much larger variance in performance and consistency, with a variance of 170.29.  
	Lot 3 that is disproportionately causing the variance at the full lot level.  




# Deliverable 3:  
## t-Tests on Suspension Coils

There is a summary of the t-test results across **all manufacturing lots**
- ![Total_summary.PNG](/Resources/Images/Total_summary.PNG)

 - From here we can see the **true mean of the sample is 1498.78**, which we also saw in the summary statistics above.  
 - With a **p-Value of 0.06**, which is higher than the common significance level of 0.05, 
 - there is **NOT enough evidence to support rejecting the null hypothesis**.  

 - Lot 1 sample actually has the **true sample mean of 1500**, again as we saw in the summary statistics above. With a **p-Value of 1**, 
 - Lot 2 has essentially the same outcome with a **sample mean of 1500.02**, a **p-Value of 0.61**; the null hypothesis cannot be rejected.
 - Lot 3 is a different scenario. Here **the sample mean is 1496.14** and the **p-Value is 0.04**, which is lower than the common significance level of 0.05.  
 - All indicating to **reject the null hypothesis** 

- ![lot_summary.PNG](/Resources/Images/lot_summary.PNG)

 - The process needs to be checked for system fails and the suspension coils from this lot need to be inspected to remove those not meeting quality criteria.

## Study Design: MechaCar vs Competition
 - There are many factors that consumers take into consideration when evaluating a car to purchase. However, 
	in a world where ridesharing is becoming more ubiquitous and it's easy and cheap to get around in other people's vehicles, 
	customers looking to purchase a car are looking for more than just a conveyance. They will be looking to buy a car 
	that is an economical means to regularly transport themselves and their items on a reliable, regular basis.
### Metric to test
 - To narrow down our test, we should evaluate MechaCar's carrying capacity, in cubic inches, in comparison to various competitors' vehicles.
### Null and Alternate Hypothesis
 - MechaCar prototypes' average carrying capacity is similar to competitor's vehicles in the same vehicle class
 - MechaCar prototypes' average carrying capacity is statistically above or below that of competitor vehicles.
### Statistical Test Used
 - The best statistical test for this would be two-sample t-tests.
### What data is needed
 - We would need to gather cubic space data from the carrying compartments of all MechaCar prototypes, as well as from all major competitor vehicles.
