# <center> Austin, Texas Dockless Vehicle Study </center>
An analysis of dockless vehicle usage in Austin, Texas related to weather <br>
![Dockless Scooter](http://s79f01z693v3ecoes3yyjsg1.wpengine.netdna-cdn.com/wp-content/uploads/2018/03/sf.Bird_.0307.jpg) 

### Project Members:
#### Petros Paterakis, Michael Alrafati, Omar Abusheikh

<hr><br>

### Overview: 

<br>

##### Is there a correlation between dockless vehicle usage & weather in Austin, TX?  

### Main Steps: 

* **Extraction** (from 2 data sources): <br>
	The [City of Austin](https://data.austintexas.gov/Transportation-and-Mobility/Dockless-Vehicle-Trips/7d8e-dm7r "City of Austin Dataset") maintains a dataset for dockless vehicle usage in the city, and this imported as a csv file into a python jupyter notebook file for further analysis.  Weather data was collected from [LSU's Souther Regional Climate Center (SRCC)](http://hrly.lsu.edu/ "Weather API") using the API which they have available; the API reponse was returned in JSON format & was imported into a jupyter notebook file. 
 
* **Transformation**: <br>
	The city of Austin dataset only contained dockless vehicle data starting on April 2018 through the present.  This data was downloaded as a csv, and was converted into a pandas dataframe.  Th   The API calls on the weather API were limited to match the city of Austin dates.  The API allowed to filter queries for specific fields & we elected to use the following fields: temp,dewp,relative_humidity,percip_1h,wind_speed,press_sea_level. API calls were return in JSON format.  
	Both datasets were converted to pandas dataframes. 
converted into pandas dataframe -> time string to datetime format for pandas to read -> transposed df to change from list of dictionaries to dictionary of lists;  
  , collecting data for every hour per day, starting on April 2018 through the present day,  to match the City of Austin dataset, 
  The time & date columns were modified to make the datasets relatable.  
  <br>
  
* **Loading**: <br>
  - Weather data was inserted into mongo db as collection via pymongo <br>
  - Dockless vehicle collection inserted into mongo database via pymongo <br>
<hr>

* **Further Potential Analysis**:
  - it would be nice to visualize the data on a map with a timeline
* **Challenges**:
  - Time format need to be rounded for the city of austin dataset
