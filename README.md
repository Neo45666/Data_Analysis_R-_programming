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




































