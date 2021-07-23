AirBnB-Data-Exploration
In this Project we have to deal with data from a well-known home rental application, named AirBnB. Specifically, we have collected data from the area of Athens for 3 months of 2019. The data is in csv format and we used Python to answer the following questions.


Question 1: Data exploration

The data given to us is organized in 3 folders (April, March, February). Each folder contains different csv files that we must combine and merge properly usingpython and pandas. In particular, we needed to create a single csv file containing the following columns:
id
zipcode
transit
Bedrooms
Beds
Review_scores_rating
Number_of_reviews
Neighbourhood
Name
Latitude
Longitude
Last_review
Instant_bookable
Host_since
Host_response_rate_rest
Bathrooms
Accommodates
Amenities
Room_type
Property_type
price
Availability_365
Minimum_nights

In this file (named train.csv) we have asked to study if there are missing data and to decide how to handle them (delete them or fill them in properly in the train.csv file). Futhermore, we have to answer the following questions using graphs, histograms, heat maps, etc. either with matplotlib or seaborn or any other library we want.

1.1) What is the most common type of room_type for your data?
1.2) Make a graph or graphs that show the development of prices for the period of 3 months.
1.3) What are the top 5 neighborhoods with the most reviews?
1.4)What is the neighborhood with the most property listings?
1.5)How many entries are per neighborhood and per month?
1.6)Draw the histogram of the neighborhood variable
1.7)What is the most common room_type in each neighborhood?
1.8)What is the most expensive room type?
1.9)Use the Folium Map library with the latitude/longitude columns and display the properties on a map for a month of your choice and in the popup map select any other information you want to appear for the property (egbed_type, room_type, transit, etc.)
1.10)Create different Wordclouds with the data from the neighborhood, transit, description, last_review.

Question 2: Recommendation System

In this query we needed the columns
Id
Name
Description.

The purpose is to extract useful information from this data and try to create a program that will generate recommendations for the area of Athens. In the first query we have already made wordclouds for the description column. In this query, we have to remove the stop words, experiment with the parameters of wordcloud and find the most characteristic words used by the visitor for the area of Athens. Then create a new column that will have the concatenation of the columns name and description (fill NA with NULL). Answer the following:
1. Create the TF-IDF (Term Frequency - Inverse Document Frequency) table of unigrams and bigrams for the new column (use the stop_word parameter of TfidfVectorizer).
2. Cosine Similarity: This metric calculates the similarity between two vectors x, y, using the angle between them (when the angle is 0 it means that x and y are equal, except for their length). Go through the TF-IDF table and calculate the similarity of each property with the rest. Save in a python dictionary the 100 most similar properties.
