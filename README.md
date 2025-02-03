# Palestinian Land Demographics GIS Automation
This is a Python project that automates geostatistical calculations and automates the creation of pie charts.

# Description & Importance

Main Goal: Reduces the amount of manual effort in ArcGIS Pro/QGIS 

Calculates the area and percentage of Palestinian Land controlled in Area A, B, H1, Nature Reserve, Gaza Strip and developed in Area C, H2, Israel Proper and East Jerusalem. 

Creates and exports interactive and non-interactive Pie Charts that illustrates the amount of land that Palestinians have developed and controlled in each West Bank governorate.

# How It's Made

Coding Languages/Libraries: Python, Pandas, GeoPandas, Matplotlib, Plotly, html2image

Data Types Supported: GeoJSON (best), other forms of spatial data such as shapefiles, geopackages (may need to make some modifications) etc...

Projection Used: EPSG:28191 Palestine 1923 / Palestine Grid

Layers Used: 
- Palestinian Land Mass
- Palestinian Seam Zone Land
- East Jerusalem Boundary
- Oslo Agreement Jurisdiction Borders
- Palestine Governorate Boundaries
- Israel Administrative Boundaries

Layer Definitions:
•	Israel Administrative Boundaries

      o This layer illustrates the Israeli District Boundaries in Israel Proper. Ex: Central District.
   
•	Oslo Agreement Jurisdiction Borders

      o	This layer illustrates land that is controlled by Palestinians in the West Bank. 
   
      o	Area A is land that is under Palestinian civil and security control.
   
      o	Area B is land that is under Palestinian civil and Israeli military control. 
   
      o	H1 is a special case in Hebron that most resembles Area A.
   
   o	H2 is a special case in Hebron that most resembles Area B, but Israelis are allowed to settle there, which is usually not the case in Area B where only Palestinians (violated in some areas) are allowed to settle and develop.
   
   o	The Nature Reserve is land that is designated as a Nature Reserve under the Wye River Memorandum which is under Palestinian civil and Israeli military control. 
   
   o	Although not included in this layer, Area C is land that is under full Israeli military and civil control with Palestinians and the majority of Israeli settlers living there. In other words, Area C is anywhere in the West Bank that        is not the Nature Reserve, Area A, B, H1, or H2. 
   
•	Palestine Governorate Boundaries

   o	This layer illustrates the Palestinian governorate boundaries in the West Bank and Gaza Strip. Ex: Jericho Governorate.
   
•	Palestinian Land Mass

   o	This layer illustrates the amount of land that Palestinians have developed in Area C, and the H2 (not including the Seam Zone), and controlled in Area A, B, H1, and the Nature Reserve. It also includes land that is developed by             Palestinians in Israel Proper and the Gaza Strip.
   
•	Palestinian Seam Zone Land

   o	This layer illustrates Palestinian land that is developed in the Seam Zone. Depending on the context, the Seam Zone can have many definitions. These definitions are as follows, any land that is in between the Green Line (West Bank         internationally recognized borders) and the West Bank barrier OR any land that is in the Jerusalem District but cut off from receiving Jerusalem municipal services in the West Bank due to the barrier OR any land that is trapped in         between an Israeli district and the West Bank barrier.
   
•	East Jerusalem Boundary

   o	This layer illustrates the East Jerusalem municipal boundary.


Where to Access/Download Layers:

[Download Data Here] (https://www.arcgis.com/home/user.html?user=MappyK)


Steps Taken:
1. Preliminary Data Exploration
   
   Gets the head of each layer
   
   Checks and changes projection of all layers to EPSG:4326 to prepare for area calculations
   
   Modifies certain attributes and field name to prepare for area calculations

   Excludes the Golan Heights
   
2. Calculate the Area in square miles of each boundary
   
   Calculated Boundaries of Israel Proper, Area A, B, H1, H2, the Nature Reserve, Gaza Strip, East Jerusalem and Area C
   
3.  Calculate the total area of Palestinian land within each of the boundaries listed above
4.  Calculate the percentage of the total area of Palestinian land within each of the boundaries
5.  Create Pie charts illustrating the amount of land that Palestinians have developed and controlled in each of the the governorates in the West Bank 
  
# Known Issues

Modifications to the data will force me to modify the code in order to reflect the changes

# Future Updates

When I finish digitizing the Israeli Land Mass layer, the pie charts as well as summary statistic data code will be updated accordingly to allow for more accurate analysis/data.
