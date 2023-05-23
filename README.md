# Eat Safe, Love

For the Eat Safe, Love challenge, the NoSql_setup file cleans and transforms the data so that it is ready for the analysis. In the NoSQL_analysis file, the data is analyzed to find the best restaurants in London. The data that was used, was the establishments.json file and it was imported into MongoDB using mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json. 

### Setup and Transformation

After importing the data and checking the formatting of the data, the next major step was to update the database with the new halal restaurant that opened and making sure that all data is correct which included updating the BusinessTypID to the correct BusinessTypeID. Next, the newspaper was not interested in any restaurants located in Dover, so all of those restaurants were removed. And finally the latitude and longitude had to be converted to decimals, and the RatingValue had to be converted to integer.

### Analysis

1. Which establishments have a hygiene score equal to 20?

There are 41 restaurants with a hygiene score of 20 acorrding to the uk_food dataset. 

2. Which establishments in London have a RatingValue greater than or equal to 4?

There are 33 restaurants with a RatingValue greater than or eqaul to 4. 

3. What are the top 5 establishments with a RatingValue rating value of 5, sorted by lowest hygiene score, nearest to the new restaurant added, Penang Flavours?

The five closest restaurants to the newly added restaurant, Penang Flavors, are: Plumstead Manor Nursery, Atlantic Fish Bar, Lumbini Grocery Ltd T/A Al-Iman, Iceland, 	Howe and Co Fish and Chips - Van 17.

4. How many establishments in each Local Authority area have a hygiene score of 0?

There 56 local autorities and here is how many each has restaurants with a hygiene score of 0:

image.png

