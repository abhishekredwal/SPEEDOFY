**Project:** Optimizing Travel Itineraries With Machine Learning


**Project goal.** The aim of my project is to expand the routes of transport vehicles using machine learning model predictions. This is a two-pronged problem: first, I train a machine learning model in data to predict how long a car will move from one place to another, and I feed this prediction into a genetic algorithm that determines which tour order works best for all given points sets.



**Data and Features.** NY city's taxi data is derived from [here](http://www.nyc.gov/html/tlc/html/about/trip_record_data.shtml), with an additional New York City weather dataset obtained from [Kaggle](https://www.kaggle.com/cabaki/knycmetars2016).

**Models.** After doing a quick foundation with a basic line breakdown on a big database I realized that a more complex model was needed. So far, I have chosen the XGBoost model that will embrace my complex features and numbers. I also used the LightGBM model when I entered the weather data because this package can handle class data and run faster, I used this model mainly for features testing.

**Optimization.** In any given set of locations, these areas are fed by a machine learning model, which predicts how long it will take to travel between two given points. The algorithm then “switches” to get a travel order that reduces the time spent traveling.

**Results.** The XGBoost model had a 4.8 minute error in estimating the length of a single car ride. While this may seem acceptable on a single trip, the error may increase when visiting multiple destinations. The genetic algorithm itself is straightforward, but it should be noted that the entire genetic algorithm provides a good balance, but not the only solution available.
