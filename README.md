# Project Name
Bike Sharing System

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. We want to understand the factors on which the demand for these shared bikes depends.
We want to identify:
1. Which variables are significant in predicting the demand for shared bikes?
2. How well those variables describe the bike demands?

## Technologies Used
matplotlib
pandas
seaborn
sklearn
statsmodels

## Observations
- there were no null values
- instant, dteday, casual, registered can be dropped based on preliminary analysis
- atemp and temp are highly corelated, one of them can be removed, we can remove atemp
- holiday, hum, weekday_sat, workinday were removed based on p-value & VIF analysis
- R-squared Value for test data is 0.80 and for train data the value is 0.83
- Adjusted R2 for test data is 0.83 and for train data the valus is 0.79
- Final model formula :
cnt = 0.2816 + 0.4302 x temp - 0.1576 x windspeed - 0.1043 x season_spring + 0.2347 x yr - 0.0460 x mnth_jan - 0.0805 x weathersit_misty + 0.0405 x season_winter - 0.0646 x mnth_jul + 0.0539 x mnth_sept - 0.0454 x weekday_sun - 0.2896 x weathersit_light_rain 

## Contact
Created by [@rahul1951991] - feel free to contact me!