# InfoViz247

This respository contains all the files and scripts that I wrote to create the 2 d3 charts for our final project -
  chart 1 - Average flight traffic of every 10 minutes a day
  chart 2 - Flight delays over a year of each airline
  
<b>Explanation of repo structure:</b>
1. index.html -- this is the index page which I place the charts
2. rawData --this folder contains all the raw data files : airports.csv & flightsOfYear.csv. I wrote three ipython notebooks to clean these data and transform them. After cleaning and transformation, 3 files were generated and put under "afterCleaning" folder
3. ReadyData -- this folder is the direct data source that I used for the visualization. I run a python script to generate the 3 files under this directory from the rawData. This step enables less computation work in javascript and gives me flexibility to construct the data in the structure that I want.
4. js -- this folder contains the two javascript files I wrote for the visualization, one for each.

<b><span style="font-size:20px;">Explanation for each chart:</span></b>


<b>Chart 1 Average flight traffic of every 10 minutes a day</b>

This chart provides visualization for the average flight traffic per 10 minutes over a day. Users can choose one of the 3 dimensions to decide what visualizations they wanna see: by City, by Airline or a Tiered dimension ( a combination of both).

When users choose one dimension, I'll use Tiered dimension as an example, the user will see a dropdown to first choose the airline he/she wants to view. After that, he will see two dropdown menus to select the city he wants to see that this airline flies two. The reason for two dropdown menus is to provide the availability to compare different cities. For example, it's a common request for a user to want to know how is the difference of traffic between Los Angeles and San Francisco for United Airline flights. The user will then be able to see the bar chart for two cities.

Similarly, the user can choose only City / Airline dimension and then select the two elements he wants to compare.

Users can freely change the dimensions.

Chart 1 Average flight traffic of every 10 minutes a day
