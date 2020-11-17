![Geekbrains Logo](https://github.com/ilyastartsdata/introductiontopython/blob/master/gb.png)

# Python libraries for Data Science. Final Project

## Real Estate Price Prediction

Geekbrains Python for Data Science course competition

> About Geekbrains: We teach people to master programming, web design and marketing from the ground up. We conduct online courses with internships and free master classes, develop the community, cooperate with employment companies and continuously test new methods to improve the effectiveness of learning.

## Overview

### Description

In this competition your task will be to predict the price of flats in test.csv. You will be given two datasets: train.csv (contains all features and prices of flats) and test.csv (only features).

### Evaluation

The evaluation metric is Coefficient of determination: R^2 = 1 - (delta)^2/(delta_y)^2

> In statistics, the coefficient of determination, denoted R2 or r2 and pronounced "R squared", is the proportion of the variance in the dependent variable that is predictable from the independent variable(s).

Source: https://en.wikipedia.org/wiki/Coefficient_of_determination

## Data

### File descriptions

- train.csv - the training set
- test.csv - the test set
- sampleSubmission.csv - a sample submission file in the correct format

### Data fields

- id - flat identification number
- DistrictId - district identification number
- Rooms - number of rooms
- Square - area
- LifeSquare - living space
- KitchenSquare - kitchen area
- Floor - floor
- HouseFloor - number of floors in the house
- HouseYear - year of construction
- Ecology_1, Ecology_2, Ecology_3 - local environmental indicators
- Social_1, Social_2, Social_3 - local social indicators
- Healthcare_1, Healthcare_2 - health-related area indicators
- Shops_1, Shops_2 - indicators related to the availability of shops, shopping centeres
- Price - flat price

## Contributing

Pull requests are welcome.

## Source

[Geekbrains](https://geekbrains.ru)
