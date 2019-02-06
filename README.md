# <center> Austin, Texas Dockless Vehicle Study </center>
An analysis of dockless vehicle usage in Austin, Texas related to weather <br>
![Dockless Scooter](http://s79f01z693v3ecoes3yyjsg1.wpengine.netdna-cdn.com/wp-content/uploads/2018/03/sf.Bird_.0307.jpg) 

### Project Members:
#### Petros Paterakis, Michael Alrafati, Omar Abusheikh

<hr><br>

### Overview: 

<br>

###### Is there a correlation between dockless vehicle usage & weather in Austin, TX?  

### Main Steps: 

* Extraction (from 2 data sources): <br>
  The [City of Austin](https://data.austintexas.gov/Transportation-and-Mobility/Dockless-Vehicle-Trips/7d8e-dm7r "City of Austin Dataset") maintains a dataset for dockless vehicle usage in the city, and this was downloaded as a csv and imported into a python jupyter notebook file for further analysis.  Weather data was collected from [LSU's Souther Regional Climate Center (SRCC)](http://hrly.lsu.edu/ "Weather API") using the API which they have available; the API reponse was in JSON format & we .   
 
* Transformation: <br>
  - Weather data will be collected 
  - Weather API as JSON response -> converted into pandas dataframe -> time string to datetime format for pandas to read -> transposed df to change from list of dictionaries to dictionary of lists;  
  , collecting data for every hour per day, starting on April 2018 through the present day,  to match the City of Austin dataset, <br>
  - We will join the datasets on dates and times. <br>
  
* Loading: <br>
  - Weather data was inserted into mongo db as collection via pymongo <br>
  - Dockless vehicle collection inserted into mongo database via pymongo <br>
