## Farm Polygon Alignment Project
# Overview
This project aligns farm polygons to match the boundaries of coffee farms using geospatial data. The process involves parsing polygon geometries from Google Sheets, performing spatial alignment operations, and saving the results back to a new Google Sheet. The project demonstrates data handling, geospatial processing, and integration with Google Sheets and GeoJSON formats.

# Features
Data Import: Fetch data from Google Sheets.

Geometry Parsing: Convert string representations of polygons into shapely Polygon objects.

Polygon Alignment: Align farm polygons with coffee farm boundaries using geometric intersection.

Export Results: Save the aligned polygons to a new Google Sheet and GeoJSON file.

Prerequisites
Python 3.x
Google Colab (for Google Sheets integration)
Required Python Libraries:
pandas
geopandas
shapely
gspread
google-auth
Setup
Authenticate Google Colab: Ensure you have access to Google Sheets by authenticating Google Colab.

Prepare Google Sheets:
Create a Google Sheet named Data with columns for geometry and Farm Polygon.

The geometry column should contain polygons in WKT (Well-Known Text) format.

The Farm Polygon column should contain polygons in a JSON-like list format.
Output

Google Sheets: A new sheet named Aligned Farm Data with the aligned polygons.

GeoJSON File: A file named aligned_farm_polygons.geojson containing the aligned polygons in GeoJSON format.

# Troubleshooting
Polygon Parsing Issues: Ensure polygon strings are correctly formatted in your Google Sheets.
Google Sheets API Errors: Verify API credentials and sheet permissions.
# License
This project is licensed under the MIT License.

# Acknowledgments
Shapely: For geometric operations.
Geopandas: For handling geospatial data.
Gspread: For Google Sheets integration.
