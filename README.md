## World Weather Analysis


# Part A: 
* I created a set of 2,000 random latitudes and longitudes in Jupyter Notebook. 
* Using the citipy module, I retrieved the nearest city and performed an API call with the Open Weather Map. 
* I retrieved and added the following information using the API call to a dataframe: latitude, longitude, max temperature, percent humidity, percent cloudiness, wind speed and weather description. 
![weather.py](https://user-images.githubusercontent.com/68629518/112195363-df914080-8bd7-11eb-9ed2-0de8efe8f25d.png) 
* The Weather_Database.ipynb and WeatherPy_Database.csv files can be found in this repo.

# Part B:  
* I imported the CSV from part A as a dataframe. 
* I wrote two input statements that would prompt the user to enter their minimum and maximum temperature criteria for their vacation. 
* Using the .loc method, I filtered the city_data_df dataframe for temperature criteria (from step above) to create another dataframe.
* I dropped any unnecessary rows that were empty or with null values.
* I created a new dataframe, hotel_df, that holds the hotel names from the hotel search above.
* There were search parameters already provided, so using them, I searched for a hotel for each city.
* I iterated the hotel_df dataframe, retrieved the latitude and longitude of each city to find the nearest hotel based on the search parameters from above. I then added the hotel name to the hotel_df dataframe. I skipped the city if a hotel isn't found.
 ![hotel_df](https://github.com/pratishthasingh1/WeatherPy/blob/master/hotel_df.png?raw=true)
* I exported the hotel_df as a CSV, which can be found in this repo under r"WeatherPy_vacation.csv."
