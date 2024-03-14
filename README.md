# Data_Analysis_R-_programming

## Background to the research

The West of England Combined Authority currently has a trial scheme in which residents can hire an e-scooter for local transport needs.
Bristol City Council are interested in potential summer demand for e-scooters based on weather, visibility, and distance from the city center. 
Data has been obtained from a city in Japan which has an e-scooter rental scheme. 
The data that has been collected from the city in Japan, is to be analysed to potentially assist Bristol City Council planning. 

## About the dataset

The data to be used is titled JapanEScooterData.csv
Examine summer days, considering only daylight hours characterized by solar radiation (MJ/m2) values greater than 0 during operational periods. Collected a sample of the subset of data for analysis, employed a number as a seed to randomly select 500 observations for this analyses. Eliminated any redundant variables where only one value remains. This refined subset of data was utilized for this analysis.
The "rented e-scooter count" is the response varibale while the other columns in the dataset represents the explanatory variables.



## Installing R- Packages

About the packages for this analysis, this can be found in the R-libraries

## 1. Data Preparation

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/124c3900-862d-4189-ba33-1f178121874a)

 Showing columns in the dataset

 ![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/e59902f3-c4c4-4a5d-bc9b-7db35f254b13)

Renaming column names

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/ce815ce2-96bb-46d8-8e63-a6d54104a1db)

Filter to retain solar radiation variables greater than zero and summer days.

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/c963b0c4-4447-4840-9caa-241402e07503)


View the structure of the dataset

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/c9066b00-7791-4f4d-aab0-b805990efece)

Remove redundant columns and select a sample of 500 observations

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/f1b33010-0c9e-4721-8730-a54c9c714e44)


# Exploratory Data Analysis

## Descriptive statistics
The appropriate descriptive statistics being the mean, median, maximum values, minimum values, first quartile and third quartile for the rented e-scooter count are numerical variables. 

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/0ce79b32-de78-46f7-ab9f-456f2fb67257)

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/4d5978f0-13d0-476a-926b-9462cd331605)

The average and median hour for rentals in the Japanese e-scooter dataset are both 13, indicating no outliers for this variable. The rental hours range from 6 to 20. The average count of rented e-scooters is 1117, with counts varying from a minimum of 9 to a maximum of 3556. During the summer period, the average temperature was 30 degrees Celsius, reaching a maximum of 41.3 degrees Celsius and a minimum of 18.7 degrees Celsius. Rainfall exhibits a wide range, ranging from a minimum of zero to a maximum of 18.5.

### Exploratory graphs
Graps explored: 
i.    Histogram
ii.   Bar plot
iii.  Scatter plot 
iv.   Line plot 

Histogram
![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/c3fc7599-2b6c-4aad-bd25-17c7b77df358)

Bar plot 
![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/4e5298d0-b7e8-4ef7-833c-f22a5d071848)

Scatter plot
![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/71d16890-21f7-445d-abd6-1ba2abe965a5)

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/4fd0d555-8b74-446f-8378-71a444b858c1)

To explore negative correlation between "rented e-scooter count" and "dew point temperature"
![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/852249aa-5db0-458a-bfa4-31c3776d10ba)

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/8938092f-d0cb-4229-8dcf-4c57f6fee8ca)

Exploring rented e-scooter count over time 

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/98bc28de-9fd5-48a8-b410-0c8dc4475fbe)

Exploration showing the box plot 

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/4de6f213-9353-4449-abf0-ad34100c6ed5)

Interpretaion of the exploratory graphs.

Histogram: The histogram illustrates the distribution of rented e-scooters, showcasing the frequency of rentals across different hours of the day. Additionally, the graph exhibits a right-skewed distribution, providing insight into the shape of the dataset.

Barplot: The barplot displays the distribution of e-scooter rentals throughout the day, indicating that the earliest rentals occur before 5 AM, while the peak rental hour is observed around the 10th hour of the day.

Scatter plot: The scatter plot reveals a positive linear relationship between the count of rented e-scooters and the hour of the day. Specifically, as the time progresses, there is an observable increase in the number of e-scooters rented. Conversely, there exists a negative relationship between the dew point temperature and the count of rented e-scooters, with higher dew point temperatures correlating with increased e-scooter rental counts.

Line Graph:
The line graph depicts the pattern of e-scooter rentals throughout the day. It reveals a positive trend wherein the number of rentals increases as the hours progress, reaching a peak before declining.

Boxplot:
The boxplot illustrates the range of values for rented e-scooters. The median, representing the middle of the box, is approximately 1000 rentals, closely aligning with the average rentals. Additionally, it delineates the interquartile range, with the first quartile ranging from 600 to the third quartile of 1500 rentals.

## Illustrating the Linear Correlation

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/a6eaa125-2cb9-425b-9a1a-44102f2ec368)

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/0084fc71-b274-47d3-9721-38349cec5b12)


![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/c254cfe6-7aaa-482e-be5e-63f2668762c1)

The variable with the most relevant linear correlation with rented e-scooter is “Hour”. It returned a value of 0.49. This shows a positive linear correlation.

## Bivariate Relationship 

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/24de6b89-5257-479a-a78a-02db3bdb6585)

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/3b71f3ce-cf80-43a3-932d-0800e7d34d1c)

Model performance evaluation and assumptions checking

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/63c1fbd8-bfd2-4f49-b740-934c907855e5)

The coefficient of determination, denoted as the multiple R-squared, is calculated to be 0.24. This implies that the model accounts for 24% of the variance observed in the rented e-scooter count. Additionally, the statistical significance of the variable "Hour" suggests that it contributes significantly to explaining the variability in the e-scooter count.

Regarding the model's performance, with an R-squared value of 0.24, it indicates that the model explains a moderate proportion of the variance in the e-scooter count. However, this leaves approximately 76% of the variance unexplained, indicating room for improvement. As for the validity of model assumptions, further diagnostics such as residual analysis and tests for normality, linearity, and homoscedasticity should be conducted to assess whether the model meets the underlying assumptions of linear regression. Subsequently, appropriate adjustments or transformations may be necessary to improve the model's fit and validity.

Further investigation

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/5d07fcac-8b97-4c52-8cce-aa604e9e3e94)

Linearity: The plot exhibits a reasonably linear relationship between the variables.
Homoscedasticity: The reference line appears relatively flat and horizontal, suggesting consistent variance across the range of predictor values.
Normality of Residuals: The distribution of residuals appears to approximate a normal shape.

Based on these observations, we can infer that the assumptions underlying linear regression have not been significantly violated.

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/af77c9d6-732d-4048-a86e-680ea803c8f5)

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/a71c602e-6c6c-47c7-be00-3cc182e11878)

The coefficient of determination, denoted as the multiple R-squared, is calculated to be 0.35. This indicates that the model accounts for 35% of the variance observed in the rented e-scooter count. Additionally, the statistical significance of the variables "Hour" and dew point temperature suggests that they both contribute significantly to explaining the variability in the e-scooter count.


## Evaluate model performance.

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/ac489ef0-614d-4bb3-95fb-c2fa7130466a)

The above graphs shows that this model validates all the assumptions of multiple regression.

## Boostraping to obtain a 95% confidence interval of the estimate of the slope

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/3ee7c966-1996-4099-be83-e3b21db1d3c2)

Show the boostrap histogram

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/68eb2558-7ad5-4b78-9fb9-bb6e85564573)


![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/f5be4787-8847-4ecb-ba91-84fac4143ef4)

# Multivariate Relationship 

Model with potential explanatory variables

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/4c8208f4-3be7-44fe-b0c6-bc6421601f22)
![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/6a1f3179-d7c1-4f55-a4f7-45f0c404d8bf)

The small general p-value indicates statistical significance for the explanatory variables, with the adjusted R-squared showing a slight increase, implying that collectively, the independent variables account for 45% of the variance in rented e-scooter counts.

The overall p-value for the model is highly significant (2.2e-16), indicating the presence of statistically significant coefficients. Specifically, "Hour", "Distance", "Dew Point Temperature", "Solar Radiation", and "Rainfall" exhibit statistical significance.

However, "Distance", "Temperature", "Wind Speed", and "Visibility" are found to lack statistical significance, suggesting that they do not contribute to the variation in e-scooter rentals within the model.

## Model evaluation

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/d9a982f4-aceb-4290-9a64-50c5a2fef7aa)
The model all the explanatory variable validates the assumption for multiple regression.

## Model simplification using Akaike Information Criterion (AIC)

It is a measure used in statistical modeling to compare the relative quality of different models. The AIC evaluates the trade-off between the goodness of fit of the model and its complexity. 

The AIC is calculated based on the likelihood function of the model and the number of parameters used in the model. It penalizes models with more parameters, thereby discouraging overfitting. The AIC value for a model is relative, meaning it is useful for comparing different models rather than providing an absolute measure of model fit.

Lower AIC values indicate better-performing models, as they achieve a good balance between model fit and complexity. When comparing models, the model with the lowest AIC is typically preferred, as it is deemed to provide the best balance between explanatory power and parsimony.

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/811792f8-8e55-4002-82f7-df4120f29227)

The model with the best balanced model is that which contails all the explanatory variables.

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/24bbcda0-9054-4e33-b600-7c2e6ca85502)
![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/de4ffed2-0797-48db-96b3-44fe0d395e24)
![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/9bb7ea74-0fda-4770-a8ad-5f0d356592c5)

The stepwise method of model selection, employing the AIC criterion, was utilized to identify the model with the lowest AIC, indicative of the best fit. Subsequent to this selection, model simplification becomes necessary to eliminate redundant variables that do not significantly contribute to the variation observed in e-scooter rentals. This process of simplification serves to reduce model complexity while enhancing accuracy.

## Evaluating model performance

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/e7994351-4785-4c1a-ba81-5ea8eb8b8d0a)

The aforementioned model indicates that each independent variable demonstrates statistical significance. Nevertheless, the R-squared value remains unchanged compared to the model encompassing all variables.

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/f8ad9d00-f170-4b63-ac57-d050b1760fe5)

The model above indicates that all independent variables exhibit statistical significance. Nonetheless, the R-squared value remains consistent compared to the model inclusive of all variables.

![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/370f99fe-7252-4bc5-a13e-9dbea6f63a85)
![image](https://github.com/Neo45666/Data_Analysis_R-_programming/assets/98716773/683f7557-bfa8-4988-9bab-d30e209fea16)

Linearity: The graph displays a linear relationship.
Homogeneity of Variance: The reference line appears flat and horizontal, indicating consistent variance.
Collinearity: There exists a linear relationship among the explanatory variables.
Influential observations: The points align along a line.
Normality of Residuals: The graphs satisfy the assumptions, with points aligning along a line and the distribution graph indicating normality.

## Report outlining findings and analyses 
