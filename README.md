# MechaCar_Statistical_Analysis

## Overview  
The purpose of this project was to run many tests and analyses on several  
datasets involving different car performances/efficiencies.  The program  
R Studio and the R programming language was used for all of the analyses.  

## Linear Regression to Predict MPG
![LnReg_to_Predict_MPG](https://user-images.githubusercontent.com/91306342/156360406-70d85dea-ee15-4c40-832e-9db49bfb1c48.PNG)  
As shown in the key above, the coefficients that significantly affected the  
MPG were vehicle weight, spoiler angle, and drivetrain. These factors explained  
about 71% of the variance in MPG according to the model, which is shown below: 

***mpg = 6.27 * vehicle_length + 1.25e-3 * vehicle_weigth + 6.88e-2 * spoiler_angle -3.41 * AWD + 3.55 * ground_clearance - 1.04e+2***  

Which can be simplified to:  
mpg = 6.27 * vehicle_length - 3.41 * AWD + 3.55 * ground_clearance - 104  
(approximate)  

## Summary Statistics on Suspension Coils

![total_summary](https://user-images.githubusercontent.com/91306342/156362855-2b7ca629-2b3a-4629-ba22-e3079baa2b97.png)  
All Locations  
![lot_summary](https://user-images.githubusercontent.com/91306342/156362898-70772dcd-5f40-4d97-939a-ac936e1dc619.png)
By each Lot  
Mechacar has in place design specs that state the variance in PSI of the  
suspension coils must NOT exceed 100 PSI. While the global variance is not  
of concern, Lot 3 has a variance much higher thann the rest and that is  
70% higher than the lowest allowable variance.  

## T-Tests on Suspension Coils
All lots vs the population mean  
![All_Lots_vs_Mean_T](https://user-images.githubusercontent.com/91306342/156364454-098fa632-fbe2-4d8f-a7f4-2e11c7be9724.PNG)  
There is not enough evidence to reject the null hypothesis- our p-value of .06  
is above the significance level of .05. This tells us the PSI across all  
lots is similar to the population mean of 1498.78 PSI.  

Individual lots  
![Lot_1_TTest](https://user-images.githubusercontent.com/91306342/156369025-c2634396-dc05-40ec-918a-c90a9428cac9.png) ![Lot_2_TTEST](https://user-images.githubusercontent.com/91306342/156369043-c21bc16d-1c06-4f4f-8bb2-006af6d3b5cc.png) ![Lot_3_TTest](https://user-images.githubusercontent.com/91306342/156369067-25e69471-30e9-400b-9cc6-46dbea59cbb2.png)
For Lot 1, the p-value is below the .05 significance level so the null hypothesis  
can be rejected. This means the PSI across the lot is statistically  
different from the population mean.  
For lots 2 and 3 the p values are above .05, so they are statistically  
similar to the population mean.

## Study Design: MechaCar vs Competition
To Compare MechaCar to the competition we have many options, for example:  

null hypothesis = Mechacar is similar to its competition in the following metrics:  
- City fuel efficiency  
- Crash-test safety ratings  
- Engine life by mileage  
- Functionality in low temperatures (starting, engine performance, etc)  








