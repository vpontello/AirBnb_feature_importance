# AirBnb Feature Importance Project

This project is the first in Udacity's Data Science Nanodegree curriculum. Its development was done using a repository on GitHub and the knowledge resulting from the project was reported through an article on Medium, which can be read [here](https://medium.com/@ing.victorpontello/this-is-why-some-accommodations-stand-out-on-airbnb-853b80e945aa).

The main objectives of this project are to train and develop communication skills with stakeholders, both technical and business ones. Therefore, for a technical audience the GitHub repository with proper documentation is the best way to communicate. For the more business-oriented audience, communication occurs through a descriptive article about what was done using the Medium platform.

## Motivation

Traveling awesome, and there is no shortage of possibilities on AirBnb, but how do you choose the right accommodation? What is the real difference between a 4.5 and a 5.0 accommodation? If I have an ad on AirBnb, what are the main points I should invest in to stand out from the other ads?.

With that said, the main motivation of the project is translated into the following research questions:

## Business Understanding

### Research Questions

1. Which are the 10 most important characteristics to influence the overall review of an acomodation?
2. What are the general differences between a top rated acomodation and a almost top one?
3. Which are the main review aspects that influences the overall review score?
4. How would be the most likely description of a acomodation in a small city like Salem, Oregon based on the findings of this study?

### Data Collection

The data which is used in this project is the AirBnb data from the following cities, and collected through this [link](http://insideairbnb.com/get-the-data.html).

To perform the analysis further information about the number of tourists of those cities gathered from [this article](https://finance.yahoo.com/news/30-most-visited-cities-u-145000465.html).

|#|City, State, Country |Foreign tourists in 2019| Population
--|--| -- | -- |
1|Asheville, North Carolina, United States|<100.000| 91560
2|Austin, Texas, United States|<200.000| 950807
3|Boston, Massachusetts, United States|1.567.000|684379
4|Chicago, Illinois, United States|1.491.000| 2710000
5|Columbus, Ohio, United States| <200.000 | 878553
6|Denver, Colorado, United States | 331.000 |705576
7|Fort Lauderdale, Florida, United States | 982.000 | 180124
8|Jersey City, New Jersey, United States | <200.000 | 261940
9|Las Vegas, Nevada, united States | 2.989.000 | 634773
10|Los Angeles, California, United States|4.645.000|3967000
11|Minneapolis, Minnesota, united States | <200.000 | 420324
12|Nashville, Tennessee, United States|<200.000|692587
13|New Orleans, Louisiana, United States|436.000| 390845
14|New York City, New York, United States | 10.288.000 | 8419000
15|Newark, New Jersey, United States | <200.000 | 281054
16|Oakland, California, United States | <200.000 | 425097
17|Portland, Oregon, United States | <200.000 | 645291
18|Rhode Island, Rhode Island, United States | <200.000 | 180972
19|Salem, Oregon, United States | <200.000 | 169259
20|San Diego, California, United States | 881.000 | 1410000
21|San Francisco, California, United States|3.308.000| 874961
22|Seattle, Washington, United States|844.000| 724305
23|Washington, D.C., District of Columbia, United States | 1.907.000 | 692683

For each city the data collected are:

1. calendar
    * listing_id
    * date
    * available
    * price

2. listings
    * id
    * listing_url
    * scrape_id
    * last_scraped
    * name
    * summary
    * space
    * description
    * experiences_offered
    * neighborhood_overview
    * notes
    * transit
    * thumbnail_url
    * medium_url
    * picture_url
    * xl_picture_url
    * host_id
    * host_url
    * host_name
    * host_since
    * host_location
    * host_about
    * host_response_time
    * host_response_rate
    * host_acceptance_rate
    * host_is_superhost
    * host_thumbnail_url
    * host_picture_url
    * host_neighbourhood
    * host_listings_count
    * host_total_listings_count
    * host_verifications
    * host_has_profile_pic
    * host_identity_verified
    * street
    * neighbourhood
    * neighbourhood_cleansed
    * neighbourhood_group_cleansed
    * city
    * state
    * zipcode
    * market
    * smart_location
    * country_code
    * country
    * latitude
    * longitude
    * is_location_exact
    * property_type
    * room_type
    * accommodates
    * bathrooms
    * bedrooms
    * beds
    * bed_type
    * amenities
    * square_feet
    * price
    * weekly_price
    * monthly_price
    * security_deposit
    * cleaning_fee
    * guests_included
    * extra_people
    * minimum_nights
    * maximum_nights
    * calendar_updated
    * has_availability
    * availability_30
    * availability_60
    * availability_90
    * availability_365
    * calendar_last_scraped
    * number_of_reviews
    * first_review
    * last_review
    * review_scores_rating
    * review_scores_accuracy
    * review_scores_cleanliness
    * review_scores_checkin
    * review_scores_communication
    * review_scores_location
    * review_scores_value
    * requires_license
    * license
    * jurisdiction_names
    * instant_bookable
    * cancellation_policy
    * require_guest_profile_picture
    * require_guest_phone_verification
    * calculated_host_listings_count
    * reviews_per_month

3. reviews
    * listing_id
    * id
    * date
    * reviewer_id
    * reviewer_name
    * comments

## Libraries used

* **pandas**: for data handling
* **numpy**: for linear algebra and numeric transformation
* **gzip**: for reading *gzip* files
* **BytesIO**: for reading IO files
* **re**: for text transforming
* **decimal**: for decimal numeric handling
* **seaborn**: for data visualization
* **matplotlib**: for data visualization
* **dataframe_image**: to convert the dataframe html output to an image
* **nltk**: for NLP sentiment analysis
* **tqdm**: for showing the loops progress while running them
* **sklearn**: for standardizing data, train test split, cross validation, and R2 score evaluation
* **lightgbm**: for ML modelling
* **xgboost**: for ML modelling

## How to explore

The project is divided in two notebooks, the first one is the **DataScience_Post.ipynb**, which was used for the data exploration and creation of the first prototypes.

However the main notebook is ProductionNotebook_AirBnb_feature_importance.ipynb, where the main methods are declared, and where the final project models were deployed.

The datasets are not versioned because of lack os storage capacity from GitHub, and the *images* directory contains some results' plots.

## Summary of the results and analysis

In this project it was found out that the most important review topic for the overall evaluation of an accomodation in AirBnb is the cleanliness, following by communication, location and check in. The top accomodations receives normally less reviews, are newer, receives less visitors, but for longer time and generate more revenue than the almost top ones. For more information about the interesting findings, please check out the [article](https://medium.com/@ing.victorpontello/this-is-why-some-accommodations-stand-out-on-airbnb-853b80e945aa).

## Acknowledgement

I would like to thank airbnb for providing the datasets used in this project. It is extremely important that real datasets are available so that the Data Science community can develop and find important insights for our society. We work for a more data driven world and by making real data available, you contribute immensely to our mission.
