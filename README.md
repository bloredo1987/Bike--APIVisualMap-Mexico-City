# Lyft Bike - API Visual Map - Mexico City
This project fetches live Mexico City bike‑share station data, converts each station into a Leaflet map marker with details, and displays everything on an interactive map so users can visually explore station locations and capacity — which is valuable for understanding bike availability and planning trips across CDMX.

# What the code does
- It downloads real-time station information from the Mexico City Lyft Bikes GBFS API using d3.json.
- It loops through each station and creates a Leaflet marker showing its location, name, and capacity using Leaflet markers.
- It groups all markers into a single layer using layerGroup.
- It builds an interactive map centered on Mexico City with OpenStreetMap tiles using Leaflet map.
- It adds a layer control so users can toggle the bike station layer on and off.

# How it shows the data
Each station appears as a clickable marker on the map. 

![alt text](<Image 3-1.png>)
Clicking a marker opens a popup with the station name and capacity. 

![alt text](<Image 2-1.png>)
The map is fully interactive — users can zoom, pan, and toggle layers.

![alt text](<Image 1-1.png>)

# Why it’s important
- It transforms raw GBFS API data into a visual, easy-to-understand map.
- Users can quickly see where stations are located and how many bikes they can hold.
- It supports real-world use cases like trip planning, capacity monitoring, and urban mobility analysis in Mexico City.

# How to Run
- Open terminal,then navigate to your project: cd ~/Desktop/'Bike Map--API Visual Map' 
- Run "python3 -m http.server 8000", leave this terminal window open 
- In your browser, go to http://localhost:8000/index.html 