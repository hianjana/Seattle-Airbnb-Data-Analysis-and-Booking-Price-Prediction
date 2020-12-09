# Seattle Airbnb Booking Price Prediction

### Project motivation

The goal behind this project is to predict the booking price of a new property in Airbnb Seattle. 
To get a better insight of the data, the below business questions are answered.

**Price overview**
How is the price distribution among all the Airbnb Seattle properties?
**Location overview**
What are the most expensive/ cheapest neighbourhoods in Seattle?
**Property type overview**
Do some property types cost more than others?
**Booking period overview**
How is the property booking per month?
Is there a peak season for Airbnb bookings?

### Data description

The files used for this project are from the open data of Kaggle: https://www.kaggle.com/airbnb/seattle

1) listings.csv - This contains the details of all the Aribnb Seattle proprty listings.
2) calendar.csv - The dates against which each listings is already booked or availabe for booking.
3) reviews.csv - The detailed reviews for each of the listing.

Since the project is aimed at new properties,the reviews.csv or any review related data present in the listings dataset has not been used. 

## Dependencies
The libraries used in the project are:

**For data pre-processing**
pandas
numpy
datetime
matplotlib.pyplot
seaborn
scipy.stats
sklearn.model_selection

**For modelling**
sklearn.linear_model
sklearn.ensemble

**For model evaluation**
sklearn.metrics


### Summary
1. Magnolia, Queen Anne and Downtown are the most expensive neighbourhoods in Seattle for Airbnb. Delridge is the cheapest one to stay.
2. Staying in a boat would be the costliest and staying in a dormitory will be the cheapest.
3. January is the peak month when it comes to bookings.
4. Summer is the peak season for bookings.
5. Random Forest model gives the best result for this data and can be used for further predictions.

### Related blog and creator info

Anjana Ambika: https://hianjana.medium.com/predict-the-booking-price-for-a-new-property-on-airbnb-seattle-83b772922e39 


