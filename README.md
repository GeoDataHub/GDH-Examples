# GDH
### How to use:  
Replace apikey section with your apikey. API keys can be acquired from https://www.geodatahub.eu/ 
For current API endpoints the key can be retrieved from here https://gdh-portal.reach-u.com.
  
### NOTE  
Current URLs do not target geodatahub.eu but instead the testing environment gdh-api.reach-u.com. Geodatahub.eu apikey will not work unless URLs are changed.

## Services  
### Web Map Service (WMS)  
Basemap service in WMS format. Contains regularly updated data layers on roads, populated places, land use, hydrography, railroads, buildings and several types of 
points of interest, shown either as pictograms (as churches, hills, rail stations, airports) or as labels (governmental and municipal institutions, schools, supermarkets etc.).

### Tile Map Service (TMS)  
Basemap service in TMS format. Contains regularly updated data layers on roads, populated places, land use, hydrography, railroads, buildings and several types of 
points of interest, shown either as pictograms (as churches, hills, rail stations, airports) or as labels (governmental and municipal institutions, schools, supermarkets etc.). 
TMS suits perfectly to web map components for fast and dynamic map display and use.

### Geocoder  
Geocode API is a service for finding geographical coordinates and structured output for entered addresses. Service analyses the input text and responds by the list of address point candidates, ordered by relevance.

### Reverse geocoder  
Reverse Geocode API is for finding readable address or place name for geographical coordinates (point location).

### Address components  
Address component service (Gazetteer) is a tool for logical and mistake-free address search and saving. The unique address objects found can be saved to client's database with all necessary attributes and coordinates.  
  
It's also possible to request address component lists by levels (e.g. all streets of a defined settlement unit).
  
### Points of Interest  
Service for finding structured attributes and geographical coordinates for points of interest (POI). Clicking on the marker will open a popup window with extra information about the selected location(Note that the data is not parsed).

### Routing Service
Route service finds the fastest route between coordinates in the supplied order.
 
### Trip Service
The trip service solves the Traveling Salesman Problem (TSP) using a greedy heuristic (farthest-insertion algorithm) for 10 or more waypoints and uses brute force for less than 10 waypoints. The returned path does not have to be the fastest path.

## Demo descriptions and usage
The demos use leaflet for displaying maps and markers. All the maps used are from GDH WMS service. First part of the code contains apikey section, where the user can enter their apikey. After that are the values that user can change to see different results. 
Lastly the urls are composed to get the right data. After that demo code is shown.
###NOTE 
GDH serves data about the Baltics so coordinates and values outside of the Baltics will not render.
### Web Map Service (WMS)  
Coordinates can be changed to display different location.
### Tile Map Service (TMS)  
Zoom level defines the zoom level of the tile. Higher zoom level renders more details. TileX and TileY define the coordinates of the tile.

### Geocoder  
User can type in address and sees a list of response candidates

### Reverse geocoder  
User can move a marker on the map and see the address of the location where the marker is placed

### Address components(Gazetteer)
User can select address components from a dropdown and see possible continuations of the address.

### Points of Interest  
Given a name of the POI displays the locations with the description on the map. The amount of POI's displayed depends on the limit. E.g query "Swedbank", with a limit 5 shows where 5 Swedbanks are located on the map.

### Routing Service
User can select two locations(By coordinates or by dragging the markers) and the shortest path between the two points is displayed

### Trip Service
In the demo user can select four locations(By coordinates or by dragging the markers) and a path that passes all the points and returns to the start is shown. Note that more markers can be used

### More info at:  
https://www.geodatahub.eu/  
https://developer.geodatahub.eu/  
