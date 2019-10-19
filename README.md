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
2. Find name of nearest city for each combination and eliminate duplicates.
3. Contact Open Weather Map API and extract weather data for city names present in API database.
4. Transform extracted weather data into Pandas data frame.
5. Export data frame to CSV file.
6. Generate scatter plot of maximum temperature data versus latitude.
7. Generate scatter plot of humidity data versus latitude.
8. Generate scatter plot of cloudiness versus latitude.
9. Generate scatter plot of wind speed versus latitude.

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

