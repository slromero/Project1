# Project 1: Food Deserts Analysis

We have two jupyter notebooks that we worked with.
The first one, named "Geoapify Places 4 Cities", is our main code, running data for our analysis.
The other one, named "Food Deserts Starter Code", is where we created our vizualizations for our data.

## Geoapify Places 4 Cities Notebook
We began by importing our dependencies, turning off warning messages, and importing the API keys.
Next, we created an instance of the census library using the year 2021, and then ran a census search to retrieve data on all zip codes from the 2021 ACS5 Census. We converted this data to a dataframe and renamed columns to be clearer, then we displayed the census dataframe.
Next, we created lists for cities and places, as well as empty lists for rows and responses, for a new supermarket dataframe.
We then ran a for loop to find supermarkets within a 10 mile radius. We set the base URL, made an API request using the params dictionary, converted the response to JSON, and then printed the response url.
Next, we ran another for loop in order to extract features and properties from JSON. Inside this for loop, we ran another for loop to extract relevant information and then printed the number of zipcodes per city.
We created the supermarket dataframe with the breakdown of zipcodes per city, and then displayed it.
We displayed information and column names for the supermarket dataframe, and then displayed the dataframe.
Once we had all this done, we created a map with the supermarkets shown.
After this, we created a new supermarket totals dataframe from the supermarket dataframe to include a column for the supermarket count for each zipcode for our cities.
We displayed the census dataframe once again, as well as information for it, and then proceeded to merge the supermarket totals and census dataframes on zipcode and displayed the new supermarkets density final dataframe.
We checked a specific zipcode to find it had no values so we changed any values of 'NaN' to '0' in the dataframe and displayed the dataframe with this change.
Next, we formatted and aggregated supermarket count by city and displayed this dataframe.
We plotted and displayed a bar chart for supermarket count by city, then we pulled the total population count by city and displayed the dataframe. Next, we plotted and displayed another bar chart for total population 2021 by city and then pulled the total poverty count by city and displayed this dataframe.
We did a merge of the city count dataframe and the population count dataframe on city and displayed the new dataframe, which we named final_two.
We calculated and displayed the number of customers per store for each city.
Then we did a merge of the final_two dataframe and the poverty total dataframe on city and displayed the new dataframe.
We then calculated and displayed the poverty percentage rate for each city.
Lastly, we added columns for poverty percentage rate and customers per store to the dataframe and displayed this final dataframe.

## Food Desert Starter Code Notebook
