# Austin_Dockless_Vehicle_Study
An analysis of dockless vehicle usage in Austin, Texas related to weather

Project Members
## Petros Paterakis
## Michael Alrafati
## Omar Abusheikh


Overview: 
City of Austin Transportation Department has recently released a dataset as part of the Dockless Mobility Service operating rules. This dataset contains information per trip and vehicle type.  Our aim is to investigate the correlation dockless vehicle usage in relation to weather. Weather data will be pulled from a public database with the help of an API.


Main Points: 

* 2 data sources: <br>
  - [City of Austin Dataset](https://data.austintexas.gov/Transportation-and-Mobility/Dockless-Vehicle-Trips/7d8e-dm7r "City of Austin Dataset") <br>
  - [Weather API](http://hrly.lsu.edu/ "Weather API") 
 
* Transformation process: <br>
  - API will be called per hour per day, since April 2018 to match Austin Dataset <br>
* Destination: <br>
  - Data will be collected & stored in database using mongo (maybe SQL)
