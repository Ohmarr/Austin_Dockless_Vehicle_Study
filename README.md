# <center> Austin, Texas Dockless Vehicle Study </center>
An analysis of dockless vehicle usage in Austin, Texas related to weather <br>
![Dockless Scooter](http://s79f01z693v3ecoes3yyjsg1.wpengine.netdna-cdn.com/wp-content/uploads/2018/03/sf.Bird_.0307.jpg) 

### Project Members:
#### Petros Paterakis, Michael Alrafati, Omar Abusheikh

<hr><br>

### Overview: 

<br>

###### The City of Austin Transportation Department maintains data related to dockless vehicle usage in the city.  
###### Our aim is to investigate the correlation between dockless vehicle usage & weather.  
###### Weather data will be pulled from LSU's Southern Regional Climate Center, which provides an API.   

### Main Points: 

* Extraction (2 data sources): <br>
  - [City of Austin Dataset](https://data.austintexas.gov/Transportation-and-Mobility/Dockless-Vehicle-Trips/7d8e-dm7r "City of Austin Dataset") <br>
  - [Weather API](http://hrly.lsu.edu/ "Weather API") 
 
* Transformation: <br>
  - We will utilitze the weather API, collecting data for every hour per day, starting on April 2018 through the present day,  to match the City of Austin dataset, <br>
  - We will join the datasets on dates and times. <br>
  
* Loading: <br>
  - Final dataset will be compiled into mongo database (maybe SQL) <br>
