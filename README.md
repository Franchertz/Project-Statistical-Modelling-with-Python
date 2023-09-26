# Final-Project-Statistical-Modelling-with-Python

## Project/Goals

### This project's objective is to examine bicycle-sharing data sourced from CityBikes, as well as location-based data obtained from Foursquare and Yelp, with the aim of uncovering valuable insights regarding the correlation between bicycle availability within a specific area and the attributes of nearby points of interest (POIs). 

## Process


### Part 1: Establishing Connection with CityBikes API: During this phase, we delved into the structure of the CityBikes API. We developed code that prompts the user for a city name and retrieves information about the chosen city. For this demonstration, Lille was selected as the city, and I successfully acquired data regarding all available bike stations, including their latitude, longitude, and the number of bikes in stock. Subsequently, I parsed the JSON data file into a Pandas dataframe.

### Part 2: 

#### Integration with Foursquare and Yelp APIs: Building on the groundwork laid in Part 1, I saved the dataframe from the initial stage as a CSV file and loaded it into the dataframe for the subsequent analysis. I established connections to the Foursquare and Yelp APIs. For each bike station, I executed queries to both APIs to amass information regarding restaurants, bars, and other specified points of interest (POIs). I generated separate dataframes to house the results from Yelp and Foursquare, allowing us to compare data quality and coverage.


### Part 3: 

#### Data Integration: In this phase, I seamlessly combined the data collected in Part 1 (bike station data) with the data obtained in Part 2 (Yelp and Foursquare results). Employing data visualization techniques, I explored the merged dataset. Furthermore, I designed and created an SQLite database meticulously considering the database structure to store the collected POI data.

### Part 4: 

#### Model Development: The final part involved the construction of a regression model utilizing Python's statsmodels library. This model aimed to scrutinize the relationship between bike availability and the characteristics of nearby points of interest (POIs). In summary, our regression analysis did not produce satisfactory results in predicting the total number of bikes based on the variables I considered. It appears that our current model may not be the optimal fit for this particular prediction task. Further investigation and potential model refinement may be necessary to enhance our predictive capabilities.



## Results

#### I have discovered that both the Foursquare and Yelp APIs offer valuable data for various purposes. My choice of which API to utilize should be guided by your specific requirements and the nature of the data you are seeking.

#### The Yelp API has proven to be particularly beneficial in my experience. It primarily provides data related to businesses and places, with a strong emphasis on user-generated reviews and ratings. This encompasses comprehensive information about businesses, such as their names, addresses, contact details, ratings, reviews, and categories. I have found it especially valuable when conducting analyses and comparisons of user opinions, ratings, and reviews for establishments like restaurants, bars, and other businesses. It is particularly well-suited for applications within the hospitality and food service industry.

#### Conversely, the Foursquare API has also played a crucial role in my work. It offers a broader spectrum of location-based data and insights that extend beyond businesses and places. In addition to business particulars, Foursquare provides data related to check-ins, user-generated tips, user profiles, and location trends. This extensive dataset has proven indispensable for exploring user behavior, monitoring trends in check-in activity, and gaining a deeper understanding of user preferences in a more general context. It stands as a versatile choice for applications that demand a comprehensive understanding of user engagement and location-based behaviors.

#### In summary, since my primary focus revolves around acquiring detailed information about businesses, their ratings, and reviews, the Yelp API was suitable option for what was required. 

## Challenges 

#### My primary hurdle revolved around deciphering the intricate nested JSON responses from the APIs to unveil their content. Along this journey, I became more adept at through the JSON response and stumbled upon some unconventional syntaxes.

#### Additionally, constructing a model presented its own set of challenges. The predicament lay in the fact that my dependent variable, 'Total Bikes,' exhibited a consistent value of zero, complicating the modeling process significantly.

## Future Goals
#### what would you do if you had more time?

#### With additional time at my disposal, I would contemplate the following avenues:

#### 1. Undertaking a more extensive analysis, utilizing larger datasets to delve deeper into the merits and limitations of each API.

#### 2. Venturing into the exploration of supplementary data sources and APIs to enhance the depth of location-based insights.

#### 3. Initiating the development of a model or recommendation system that harnesses the amalgamated data from multiple sources, with the goal of enhancing the precision of location-based recommendations.

#### This project serves as a cornerstone for future endeavors in the realms of comprehensive research and application development within the domain of location-based data analysis and the modeling of user behavior.
