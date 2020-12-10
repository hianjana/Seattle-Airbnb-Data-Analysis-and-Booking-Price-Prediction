# Seattle Airbnb Booking Price Prediction

This project uses the Airbnb Seattle open data available on Kaggle. The data is from April 2016 to February 2017 which is 11 months data.

## Table of Contents

- [Motivation](#motivation)
- [Overview of data](#overview-of-data)
- [High level data preparation steps](#high-level-data-preparation)
- [Modelling techniques used](#modelling-techniques-used)
- [Summary](#summary)
- [Related blogs and creator info](#related-blogs-and-creator-info)

## Motivation

The goal behind this project is get a business understanding on the data and also to predict the booking price of a new property in Airbnb Seattle. Apart from predicting the booking price of a new property, the project explores the below areas:

1. Price overview
2. Location overview
3. Property type overview
4. Booking period overview
5. Booking price prediction

## Overview of data

The repository contains the following files:

    ├── README.md
    ├── calendar.zip
    ├── listings.zip
    ├── seattle_airbnb.ipynb

The files used for this project are from the open data of Kaggle: https://www.kaggle.com/airbnb/seattle

1) listings.zip - This zip file contains the details of all the Aribnb Seattle proprty listings.
2) calendar.csv - This zip file contains the dates against which each listings is already booked or availabe for booking.

Since the project is aimed at new properties,the reviews.csv or any review related data present in the listings dataset has not been used. 


## High level data preparation steps

These are the high-level steps taken for data cleaning:
1. Remove data that doesn’t vary (drop columns with the same value).
2. Remove data that are 100% unpopulated (drop columns with all null values).
3. Replace unpopulated data with mean/ mode (Fill nulls with the mean for numerical and mode for categorical columns).
4. Add meaningful new data using existing ones (Add new columns using some existing columns).
5. Drop irrelevant data (Since review information is not required, all review related columns are dropped. Since text mining is not used, all columns 
   with heavy text are dropped, and also url information are not required).

## Modelling techniques used

One linear model and one ensemble model are used in this project.
- Linear Regression
- Random Forest Regressor

The models are evaluated using:
- Mean Squared Error
- R2 Score

## Summary

1. Magnolia, Queen Anne and Downtown are the most expensive neighbourhoods in Seattle for Airbnb. Delridge is the cheapest one to stay.
2. Staying in a boat would be the costliest and staying in a dormitory will be the cheapest.
3. January is the peak month when it comes to bookings.
4. Summer is the peak season for bookings.
5. Random Forest model gives the best result for this data and can be used for further predictions.

## Related blogs and creator info

Anjana Ambika

- Technical blog: https://hianjana.medium.com/predict-the-booking-price-for-a-new-property-on-airbnb-seattle-83b772922e39 
- Business overview blog: https://hianjana.medium.com/making-the-best-out-of-airbnb-seattle-data-d6c7533a6286


