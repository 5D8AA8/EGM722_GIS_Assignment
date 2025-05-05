Terrorism Mapping Tool (TMT)

This notebook-based GIS tool was built as part of the EGM722 Programming for GIS and Remote Sensing module at Ulster University. It lets users load, clean, and map incident data (such as terrorism events) and view them interactively using Folium. The idea was to make something usable and understandable, especially for someone still learning Python and GIS like me.

What it does

- Loads and cleans CSV and shapefile data
- Projects points on a map
- Identifies bounding boxes and shapes
- Connects to NASA EarthData using EarthAccess
- Downloads and displays satellite imagery

Getting Started

To run this, either clone or download it as a ZIP. Then,

1. Install the environment with:
   conda env create -f environment.yml
   conda activate tmt
   jupyter notebook

2. Open the GIS_Assigment.ipynb file.
3. Follow the steps cell by cell, comments and markdown are included to explain what’s happening.

Common Issues

- Some map shapes not showing? Try:
  gdf['geometry'] = gdf['geometry'].buffer(0)

- If the file dialog doesn’t show up, make sure you’re running this with a GUI (not headless).

Credits

This was developed as part of a coursework submission and learning exercise. 

See the full User Manual in the repository for more detail and screenshots.
