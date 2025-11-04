# GeoJsonVisual

A minimal, responsive web app for visualizing GeoJSON datasets on an interactive map using Leaflet.js. Easily explore spatial data such as recent DC crime incidents, US state boundaries, and more.

## Features
- Interactive map with Leaflet.js
- Visualizes GeoJSON points and polygons (e.g., crime incidents, state boundaries)
- Color-coded markers and polygons by data attributes (e.g., crime type, obesity rate)
- Sidebar with sortable, clickable data table
- Popups with detailed information on map features
- Responsive, mobile-friendly UI
- Easily switch datasets by editing the loader in `index.html`

## Local Usage
1. Clone or download this repository.
2. Place your GeoJSON files in the `assets/` folder.
3. Open `index.html` in a web browser, or run a local server for full functionality:
   
   ```powershell
   python -m http.server
   ```
   Then visit [http://localhost:8000](http://localhost:8000) in your browser.

## Datasets
- `assets/crime30days.geojson`: DC crime incidents (last 30 days)
- `assets/dc.geojson`: Washington DC boundary
- `assets/earthquakes.geojson`: Example earthquake data
- `assets/japan.json`: Example Japan data

## Japan Earthquake Visualization

The project includes an additional page, `earthquake.html`, which visualizes earthquake data in Japan using the `assets/japan.json` GeoJSON file. This page demonstrates how to:
- Display point data for earthquakes with magnitude-based color and size
- Show popups with earthquake details (magnitude, location, date)
- Interactively explore seismic activity in Japan

To use:
1. Open `earthquake.html` in your browser (or via your local server)
2. Explore the map and click on earthquake points for more information

You can use this page as a template for other point-based GeoJSON visualizations.

## Customization
- To visualize a different dataset, update the loader function in `index.html` to point to your GeoJSON file and adjust the popup/table logic as needed.
- Color scales and legends can be customized in the script section.

## Dependencies
- [Leaflet.js](https://leafletjs.com/) (loaded via CDN)
