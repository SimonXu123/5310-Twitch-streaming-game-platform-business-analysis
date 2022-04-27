# Project description
## Project background:

In order to continue expanding the market share, it is common for streaming platforms to buy out exclusive broadcast rights of some most welcomed video games. Therefore, it becomes crucial to successfully predict their popularity, and then to make further business decisions based on that prediction.

## Project outline

The goal of this report is to evaluate the potential commercial value of video games by testing whether the stream performances at peak time(peak viewers and peak channels in the specific games) have a significant effect on the total game popularity.

## Project method(R programming)

1. Used read.csv() to read the original  data file
2. Applied scatterplot matrix() to show different relations of attributes
3. used lr() function to build multilinear regression models
4. used stepAIC() function to choose the best multiple linear regression model between the complete model and the reduced model. And the best regression model is Hours_Streamed + Streamers + Peak_viewers + Peak_channels are independent variables to the Hours_watched.

## Project result:

The above statistical analyses have proved the importance of the data regarding two peak indices for linear regression model fitting optimization. It is sufficient to show that the two peak variables are significantly correlated to the hours watched when the average viewers are not given.

1. For example, increasing an additional 100 viewers at the peak time leads to an increase in the total hours of the watch by approximately 61*100 = 6100 hours on average. The R-squared represents the correlation coefficient between the observed values of the outcome variable (y) and the fitted (i.e., predicted) values of y.
2. R-squared value of closing to 1 indicates that the model explains alarge portion of the variance in the outcome variable. The R-squared is 0.7442, meaning that 74% of the variance in the measure of hours_watched can be predicted by hours streamed, peak viewers, peak channels, streamers, and average viewers. Overall, the evaluation result for our predicted model is acceptable as each predictor shows a closed relationship to the dependent variable.
