# Palestinian Land Demographics GIS Automation
This is a Python project that automates geostatistical calculations and automates the creation of pie charts.

# Description & Importance

Main Goal: Reduces the amount of manual effort in ArcGIS Pro/QGIS 

Calculates the area and percentage of Palestinian Land controlled in Area A, B, H1, Nature Reserve, Gaza Strip and developed in Area C, H2, Israel Proper and East Jerusalem. 

Creates and exports interactive and non-interactive Pie Charts that illustrates the amount of land that Palestinians have developed and controlled in each West Bank governorate.

# How It's Made

Coding Languages/Libraries: Python, Pandas, GeoPandas, Matplotlib, Plotly, html2image

Data Types Supported: GeoJSON (best), other forms of spatial data such as shapefiles, geopackages (may need to make some modifications) etc...

Projection Used: EPSG:4326 

Layers Used: 

Layer Definitions:

Where to Access/Download Layers:

Steps Taken:
1. Preliminary Data Exploration
   
   Gets the head of each take
   
   Checks and changes projection of all layers to EPSG:4326 to prepare for area calculations
   
   Modifies certain attributes and field name to prepare for area calculations
3.  
  
# Known Issues

Modifications to the data will force me to modify the code in order to reflect the changes

# Future Updates

When I finish creating the Israeli Land Mass layer, the pie charts as well as summary statistic data code will be updated accordingly to allow for more accurate analysis/data.
