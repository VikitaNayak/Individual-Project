# Individual-Project
## Individual Project Part 1 - Data Exploration

### Individual Project Objective :

-  #### Transform an unknown dataset into visualizations. 
            This activity will allow you to learn from how to explore data and iteratively develop effective visualizations.
-  #### Get comfortable using Tableau. 
            Tableau is an important tool for data visualization. Completing the individual project will provide you with the skills to comfortably use Tableau.


### Dataset used for this project:  City of Chicago’s Automated Speed Enforcement Program. 
https://data.cityofchicago.org/Transportation/Speed-Camera-Violations/hhkd-xvj4

#### Details of the dataset
- ADDRESS: Address of the location of the speed enforcement camera(s). There may be more than one camera at each address.
- CAMERA ID: A unique ID associated with the physical camera at each location. There may be more than one camera at a physical address.
- VIOLATION DATE:	The date of when the violations occurred. NOTE: The citation may be issued on a different date.
- VIOLATIONS: Number of violations for each camera on a particular day
- X COORDINATE: The X Coordinate, measured in feet, of the location of the camera. Geocoded using Illinois State Plane East (ESRI:102671).
- Y COORDINATE: The Y Coordinate, measured in feet, of the location of the camera. Geocoded using Illinois State Plane East (ESRI:102671).
- LATITUDE: The latitude of the physical location of the camera(s) based on the ADDRESS column. Geocoded using the WGS84.
- LONGITUDE: The longitude of the physical location of the camera(s) based on the ADDRESS column. Geocoded using the WGS84.
- LOCATION: The coordinates of the camera(s) based on the LATITUDE and LONGITUDE columns. Geocoded using the WGS84.

This dataset reflects the daily volume of violations that have occurred in Children's Safety Zones for each camera. The data reflects violations that occurred from July 1, 2014 until present, minus the most recent 14 days. This data may change due to occasional time lags between the capturing of a potential violation and the processing and determination of a violation. The most recent 14 days are not shown due to revised data being submitted to the City of Chicago. The reported violations are those that have been collected by the camera and radar system and reviewed by two separate City contractors. In some instances, due to the inability the registered owner of the offending vehicle, the violation may not be issued as a citation. However, this dataset contains all violations regardless of whether a citation was issued, which provides an accurate view into the Automated Speed Enforcement Program violations taking place in Children's Safety Zones.

##### NOTE: This data gives us speed camera violation information in areas of chicago. When this dataset combined with other dataset such as accident in chicago then it can give us good insights to find whether the major accident occuring in the Children's safety zones of chicago are due to speed violations. We can find reasons causing the accident and can take preventive actions to reduce number of accidents.


#### Develop 5 distinct visualization using Tableau that provide an effective overview of the data

#### Visualization 1 

- This graph shows the trend of speed violations over the period of 2014 to 2019 in Chicago. 
- From the graph, it seems that the number of speed violations increased drastically from 2014 to 2015 and are at its peak during the year of 2015. 
- After 2015, the number of violations started decreasing gradually in the years of 2016, 2017, 2018 and 2019.
- Here, the red color shows highest number of violation and green shows lowest number of violations
- This graph is simple line chart showing the trend of speed violation and can be helpful for someone who just wants an overview of the speed vilations. The columns used to create this chart are 'Year of Violation Date' and 'Violations'.
- This graph shows a positive sign that the number of violations are decreasing in Chicago

![image.png](attachment:image.png)

#### Visualization 2
- This is a map of chicago representing the areas and the number of speed camera violations occured for that area
- The dark red circle indicates highest number of speed camera violation area
- The light green circle indicates least number of speed camera violation area
- This map representation is helpful to identify the areas of speed camera violations
- The Year filter is provided to check the spped violation number of an area per year

![image.png](attachment:image.png)

#### Visualization 3
- This visualization is a bubble chart which shows top 20 Speed violations by Address & Camera Ids 
- This visualization displays granular level details of the above map represenatation (Visualization 2) 
- The columns used to create 1st graph are 'Address','Camera Id' and 'Violations'
- This visualization also provides filter of Year where we can see top 20 violation for any year(2014-2019) by Camera Id and Address
- The address or camera ids with highest number of violations are in red and lowest number of violations are in dark green
- The filter of Year is also provided  for more granularity which can be used to see violations for each year by Address or Camera ids

![image.png](attachment:image.png)

#### Visualization 4

- This is a bar graph which shows some more granular details as compared to the above graph(Visualization 3)
- It shows the average number of speed violations monthly trend for each year(2014 - 2019)
- Here, the average violation number is decreasing over the yearly period of 2014 to 2019
- The monthly trend(in each year) shows that the average speed violation number start increasing in the month of July and gradually decrease till december.
- The columns used to create this graph are 'Violation Date' and 'Violations'
- The red color shows the high number of violations and green shows low number of violations

![image.png](attachment:image.png)

#### Visualization 5

- This is a heat map showing Speed Camera Violation by Days and Month for the year 2014 - 2019

- #### Monthwise Observation :
    - Overall, it can be said that the number of Speed Camera Violations drastically increased in the month of July ( may be due to summer vacation when more people like to travel with their families)
    - Also, we observe high number of violations inthe month of September, October, November and December (As we have holidays during this period, people might be travelling more)
    - The violation numbers are low in the month of January & February ( No holidays, lesser number of people travelling)
- #### Daywise Observation :
    - It seems the Friday is the day when maximum speed camera violations occurs for mostly all the months
    - It is also important to note that Friday is the day in all the months where high number of speed Violation occurs
        - For example, high number of speed violations occured in the month of July, September,October, November & December and corresponding Fridays also have the high number of speed violations for these months.
        
- #### Overall Observation:
- This heat map gives us a lot of details by providing number of violations for each year, month and weekdays.
- This information can be helpful to predict days in future when speed violations will be high and necessary steps can be taken this information is combined with the accident in chicago dataset to find whether the accidents occuring in Chicago are due to the speed violations or not.
     

![image.png](attachment:image.png)

### Conclusion

- Each visualization is different from each other and provides details at high level (Visualization 1) to very detailed level (Visualization 5)
- Visualization 1 is a line chart which gives a very high level information about the trend of the speed violations in Chicago from 2014 to 2019
- Visualization 2 is a map representation which is a bit granular than Visualization 1 and gives information about the speed violations occured in different areas of Chicago and this can be filtered using Year filter
- Visualization 3 is a bubble chart which shows top 20 Address or camera ids where number of speed violations are high and this can be filtered by Year as well. 
- Visualization 4 is a bar chart which gives more details about average speed violations occuring per month of each year.
- Visualization 5 is heat map which gives detailed level information about speed violations occuring per day per month of each year
- Here, the color code is uniform in all the graphs where red indicates high number of speed violations and green represents low number of speed violations.
- The graphs have Year filters to provide more granularity
- The important descriptors of the dataset are the columns :  Violations, Longitude, Latitude, Camera Id,Violation Date and Address-
- The speed violations has beed decreased over the period of time from 2014 to 2019
- This data analysis can be helpful for police department of Chicago. This can be looked together with the accident dataset to find whether the accidents are occuring due to speed violations

