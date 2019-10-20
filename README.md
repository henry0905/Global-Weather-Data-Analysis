# Global-Weather-Data-Analysis

The goal of this project was to analyze weather data related to maximum temperature, humidity, wind speed, and cloudiness for over 500 randomly selected global cities. Since the baseline data was collected from the Open Weather Map API, Python with Numpy, Citipy, Requests, Pandas, and Matplotlib (through Jupyter Notebooks) was used to clean and process the data, as well as display the desired outputs.

## Questions

1. Is a correlation present between latitude and maximum temperature? If so, what is the nature of that relationship?
2. Is a correlation present between latitude and humidity? If so, what is the nature of that relationship?
3. Is a correlation present between latitude and wind speed? If so, what is the nature of that relationship?
4. Is a correlation present between latitude and cloudiness? If so, what is the nature of that relationship?

## Datasets

1. https://github.com/mjknj18/Global-Weather-Data-Analysis/blob/master/Global%20Weather%20Data/Global_Weather_Data.csv

## Tasks

1. Generate 2000 random latitude and longitude combinations.
2. Find the name of the nearest city for each combination and eliminate duplicates.
3. Contact the Open Weather Map API and extract weather data for city names present in the API database.
4. Transform the extracted weather data into a Pandas data frame.
5. Export the data frame to CSV file.
6. Generate a scatter plot of maximum temperature data versus latitude.
7. Generate a scatter plot of humidity data versus latitude.
8. Generate a scatter plot of wind speed data versus latitude.
9. Generate a scatter plot of cloudiness data versus latitude.

## Results

### City Latitude Versus Maximum Temperature

<img src = https://github.com/mjknj18/Global-Weather-Data-Analysis/blob/master/Images/City_Latitude_vs_Maximum_Temperature.png>

### City Latitude Versus Humidity

<img src = https://github.com/mjknj18/Global-Weather-Data-Analysis/blob/master/Images/City_Latitude_vs_Humidity.png>

### City Latitude Versus Wind Speed

<img src = https://github.com/mjknj18/Global-Weather-Data-Analysis/blob/master/Images/City_Latitude_vs_Wind_Speed.png>

### City Latitude Versus Cloudiness

<img src = https://github.com/mjknj18/Global-Weather-Data-Analysis/blob/master/Images/City_Latitude_vs_Cloudiness.png>

## Observations

Examining the maximum temperature data, there is a clear trend showing a drop in temperature the farther a city is located from the equatorial region. The scatter plot is flat between the latitudes of -20 and 20, but then drops off roughly evenly in both directions until the latitudes of -60 and 60. Beyond that point, it can be assumed that this trend continues to both polar regions, but there is not sufficient data approaching the Antarctic region of the southern hemisphere. This trend is explained by the curvature and tilt of the Earth. The equatorial regions are at the widest part of the planet and aren't as affected by Earth's curvature and tilt relative to the sun. Therefore, they receive more consistent sunlight all year long, which results in higher maximum temperatures. In contrast, cities farther to the north or south receive less sunlight due to the curvature and tilt, which results in lower maximum temperatures.

In regard to the humidity and wind speed data, it is evident that the majority of cities have humidity percentages above 60 percent and wind speeds below 15 miles per hour. In both cases, the scatter plots show the data primarily grouped in those zones, regardless of latitude. Humidity percentages are more likely tied to the climactic region of a particular city and specific weather patterns in that area. Wind speeds could be tied to a city's altitude, surrounding geographical/physical features, and/or current weather systems.

Reviewing the cloudiness data, there is no clear correlation present with respect to latitude. The scatter plot shows a near even distibution of data throughout, although there are some small groupings present. Cloudiness is more dependent on a city's daily weather. For example, a rainy or snowy day would more likely have a higher cloud percentage, while a sunny day would generally have a lower percentage.