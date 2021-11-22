# Simulations

Created so that we could examine just the effect of age and time on four categories: normal, low baseline, rapid decline, and low baseline rapid decline.

## Parameters around the normal:
1. Age from 20 to 90.
2. White female 160cm
3. Using NHANES3 equations, then 
fev1<- 0.4333-0.00361*age-0.000194*age^2+0.00011496*height^2
4. FEV1 standard deviation for sampling at each time point was 0.4, e.g. the value at each time point was selected from a normal distribution with a mean representing the actual value and the standard deviation representing the SD.

## Parameters for low baseline and rapid decline
1. Low baseline has an FEV1 that is 0.25 less at each time point
2. Rapid decline has a FEV1 that is 0.01 less per each year.

## Linear approximation (these models say "L")
Using the best fit of the original prediction we get
fev1L<- 0.4333-0.01773*age+0.00011496*height^2

Further details can be found in the simulations.rmd file
