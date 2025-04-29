# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goal of this project was to explore the relationship between bike availability at public stations and the proximity of points of interest (POIs), using real-time data.
I also aimed to evaluate the quality of POI data retrieved through both the Yelp API and the Foursquare API, and to build predictive models using regression and classification techniques.

## Process
### Data Collection:
- Collected bike-sharing data (free bikes) from a public API.
- Fetched POI data using Yelp API and Foursquare API, based on the coordinates of bike stations.

### Data Cleaning and Merging:
- Cleaned, filtered, and merged bike data with POI data.
- Engineered new features such as venue_distance (distance between station and nearby venue).

#### Exploratory Data Analysis:
- Analyzed patterns between bike availability and POI proximity.
- Visualized relationships and distributions to guide modeling.

##### Modeling:
- Performed a linear regression analysis to predict the number of free bikes using venue_distance.
- Built a logistic regression model to classify bike availability into categories: Low, Medium, and High.

## Results
# API Coverage:
Both Yelp and Foursquare provided valuable POI information. However, there were variations in data quality, with Foursquare often providing more detailed or categorized venue data.

# Regression Model:
Found a statistically significant but weak relationship between distance to POIs and bike availability.

# Classification Model:
Logistic regression provided moderate classification performance. It showed that venue_distance alone has some predictive power, but other features would improve the model.

## Challenges 
- Managing API key security (keeping keys outside the notebook and safe).
- Handling missing or inconsistent POI information from both APIs.
- Dealing with the limited predictive power of a single feature (venue_distance) without richer contextual data.
- Merging datasets coming from two different APIs with different formatting and standards.

## Future Goals
- Incorporate additional features like weather conditions, time of day, and special events to improve model accuracy.
- Compare other machine learning models (Random Forest, XGBoost, SVM).
- Build a model that uses both Yelp and Foursquare POI features together.
- Expand analysis across different cities and over longer time periods to strengthen findings
