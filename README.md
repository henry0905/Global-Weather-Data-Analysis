# Global-Weather-Data-Analysis

The goal of this project was to analyze weather data related to maximum temperature, humidity, cloudiness, and wind speed for over 500 randomly selected global cities. Since the baseline data was collected from the Open Weather Map API, Python with Numpy, Citipy, Requests, Pandas, and Matplotlib (through Jupyter Notebooks) was used to clean and process the data, as well as display the desired outputs.

## Questions

1. Is a correlation present between latitude and maximum temperature? If so, what is the nature of that relationship?
2. Is a correlation present between latitude and humidity? If so, what is the nature of that relationship?
3. Is a correlation present between latitude and cloudiness? If so, what is the nature of that relationship?
4. Is a correlation present between latitude and wind speed? If so, what is the nature of that relationship?

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
8. Generate a scatter plot of cloudiness versus latitude.
9. Generate a scatter plot of wind speed versus latitude.

## Results

### City Latitude Versus Maximum Temperature

<img src = https://github.com/mjknj18/Global-Weather-Data-Analysis/blob/master/Images/City_Latitude_vs_Maximum_Temperature.png>

### City Latitude Versus Humidity

<img src = https://github.com/mjknj18/Global-Weather-Data-Analysis/blob/master/Images/City_Latitude_vs_Humidity.png>

### City Latitude Versus Cloudiness

<img src = https://github.com/mjknj18/Global-Weather-Data-Analysis/blob/master/Images/City_Latitude_vs_Cloudiness.png>

### City Latitude Versus Wind Speed

<img src = https://github.com/mjknj18/Global-Weather-Data-Analysis/blob/master/Images/City_Latitude_vs_Wind_Speed.png>

## Observations

The purpose of this assignment was to analyze current weather data from over 500 randomly selected global cities. The Numpy, Citipy, Requests, Pandas, and Matplotlib modules in Python were used to generate random latitude and longitude combinations, generate the city name and extract weather data from the Open Weather Map API for each combination, process that data to find certain metrics, and generate plots to display meaningful results. This allowed for several observations to be made from the data regarding how maximum temperature, humidity, cloudiness, and wind speed vary based on a city's latitude.

Looking at the maximum temperature data, there is a clear trend showing a drop in temperature the farther a city is located from the equatorial region. The scatter plot flattens out between the latitudes of -20 and 20, but then drops off evenly in both directions until the latitudes of -60 and 60. Beyond that point, there is strong evidence that this trend continues to the polar regions, but there is not sufficent data for the lower portions of the southern hemisphere. An explanation of this trend comes from the curvature and tilt of the Earth. The equatorial regions are at the widest part of the planet and aren't affected as the Earth tilts about that axis. Therefore, they recieve more consistent sunlight, which results in a higher maximum temperature. In contrast, the Earth's tilt causes cities farther to the north or south to recieve less consistent sunlight, which results in a lower maximum temperature.

Looking at the humidity and wind speed data, it is evident that the majority of cities have humidity percentages above 60 percent and wind speeds below 15 miles per hour. In both cases, the scatter plots show the data primarily grouped in those regions, regardless of latitude. Humidity percentages are more likely tied to the climactic region of a particular city, such as the amount of yearly rainfall and/or its location relative to large bodies of water. Wind speeds are more likely tied to a city's altitude and/or surrounding geographical features, as these would determine whether a city is shielded from or exposed to high wind speed events.

Looking at the cloudiness data, there is no clear correlation present with respect to latitude. The scatter plot shows an even distibution of data throughout, although there are some slighly larger groupings present. The cloudiness is probably more dependent on the daily weather patterns a city experiences. For example, a rainy or snowy day would have a larger cloud percentage, while a sunny day would have a lower percentage.