# Project 1: Food Deserts Analysis

We used a Google Doc for our collaboration:
https://docs.google.com/document/d/1ZLTZfn4TfGabZN2vWS41wqPgEh_MCRO0MjD5_WTs9mk/edit?usp=sharing

We also used a Google Presentation for our presentation:
https://docs.google.com/presentation/d/1qbKaD6DTTfHBibHcoHtcd6msB4QAEu6V-_ABy75_HCY/edit?usp=sharing

We have two jupyter notebooks that we worked with.
The first one, named "Geoapify Places 4 Cities", is our main code, running data for our analysis.
The other one, named "Food Deserts Starter Code", is where we created our vizualizations for our data.

## Geoapify Places 4 Cities Notebook

We began by importing our dependencies, turning off warning messages, and importing the API keys.
Next, we created an instance of the census library using the year 2021, and then ran a census search to retrieve data on all zip codes from the 2021 ACS5 Census. We converted this data to a dataframe and renamed columns to be clearer, then we displayed the census dataframe.
Next, we created lists for cities and places, as well as empty lists for rows and responses, for a new supermarket dataframe.
We then ran a for loop to find supermarkets within a 10 mile radius. We set the base URL, made an API request using the params dictionary, converted the response to JSON, and then printed the response url.
Next, we ran another for loop in order to extract features and properties from JSON. Inside this for loop, we ran another for loop to extract relevant information and then printed the number of zipcodes per city.
We created the supermarket dataframe with the breakdown of supermarkets per city, and then displayed this information.
We then displayed the supermarket dataframe.
Once we had all this done, we created a map with the supermarkets shown.
After this, we created a new supermarket totals dataframe from the supermarket dataframe to include a column for the supermarket count for each zipcode for our cities.
We then proceeded to merge the supermarket totals and census dataframes on zipcode and displayed the new supermarkets density final dataframe.
We checked a specific zipcode to find it had no values so we changed any values of 'NaN' to '0' in the dataframe and displayed the dataframe with this change.
Next, we formatted and aggregated supermarket count by city and displayed this dataframe.
We then formatted and aggregated total population count by city and displayed this dataframe.
We did a merge of the city count dataframe and the population count dataframe on city and displayed the new dataframe, which we named final_two.
We plotted and displayed a bar chart for supermarket count by population per city.
After this, we formatted and aggregated total poverty count by city displayed this dataframe.
Then we did a merge of the final_two dataframe and the poverty total dataframe on city and displayed the new dataframe called final_three.
We then calculated and displayed the poverty percentage rate for each city.
Lastly, we added a column for poverty percentage rate and customers per store to the dataframe and displayed this final dataframe.

## Food Desert Starter Code Notebook

We began by importing our dependencies and loading the csv data.
We filtered for specific counties that we chose to look into more and renamed a column in the csv to be more recognizable as a food desert.
We added map colors on the graph, then created a vertically stacked bar chart, setting labels and the title, as well as customizing legend labels, rotating the x-axis labels to be horizontal.
We printed the numeric values and added a legend assigning each color to being a food desert (yes) or not being a food desert (no), then we showed the plot.
Next, we created a for loop to loop through each county and created pie charts showing the distribution of food deserts in each county. We displayed all four pie charts in one plot.
Then we created a for loop to loop through each county and created bar charts showing food deserts for urban vs in each county, which we displayed in separate bar chart plots for each county. We also displayed a summary of the total population for each county based on food desert with a breakdown of it is a food desert or not above each bar chart plot.
Then we created a for loop to loop through each county and created bar charts showing food deserts by urban vs non-urban in each county, which we displayed in separate bar chart plots for each county, with two bars per bar chart plot. We also displayed a summary of urban vs non-urban counts for each county above all the bar chart plots.
Lastly, we created a for loop to loop through each county and created scatter plots for food desert vs poverty rate, which we displayed in separate scatter plots for each county.