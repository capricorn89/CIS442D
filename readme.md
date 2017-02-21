# Basemap Tutorial

## Motivation
The Basemap toolkit (URL: http://matplotlib.github.com/basemap/ ), an add-on to matplotlib, enables plotting 2D data on maps in Python. 
The main objective of basemap toolkit is to provide globe projections by transforming projecting latitude and longitude coordinates on the globe onto a two-dimensional Matplotlib plot. 
Contours, images, vectors, lines, or points can be plotted in Matplotlib, which is then used to display roads, shoreline, river, coastline, or any kinds of boundary datasets from various generic mapping tools such as ArcGIS mapping programming.
Therefore, the basemap library can give desired map projection region in user-friendly manner. 
This 2D map projection feature can satisfy various needs, such as climate and weather forecasting, future earthquake research, oil and gas detection, or any subject area that requires detailed observation of globe with high accuracy as well as clear readability of projected map region produced by the basemap.


## Context - alternative solutions for solving the problem

### Representative Map Expression Library
- cartopy: a cartographic python library with matplotlib support for visualisation. Cartopy is a Python package designed to make drawing maps for data analysis and visualisation easy.
- googlemaps : python client library for Google Maps API Web Services.
- folium : this makes it easy to visualize data that’s been manipulated in Python on an interactive Leaflet map. It enables both the binding of data to a map for choropleth visualizations as well as passing Vincent/Vega visualizations as markers on the map.
- geoplotlib: python toolbox for geographic visualizations
- vincent: this takes Python data structures (tuples, lists, dicts, and Pandas DataFrames) and translates them into Vega visualization grammar. It allows for quick iteration of visualization designs via simple addition and subtraction of grammar elements, and outputs the final visualization to JSON.

### Essential library for geospatial problem solving
- pandas: For data handling and munging. This is tool for working with data in a spreadsheet-like format. 
- shapely: For geometry handling. This is the package for geometry handling and manipulation.
- rtree: For efficiently querying spatial data. This is a relatively simple spatial index package that speeds up spatial bounding box queries.
- nodebox-opengl: For creating and controlling animations. This package makes it easy to create some simple, interactive animations.
- statsmodels: For models and stats in Python. It enables user to use statistical approach in python.    
- numpy: For dataset in arrays. This is useful package for data analysis in python. 
- geopy: For geolocating addresses. It is a small wrapper around various web-based geocoding APIs.
- ipython: For interactive Python environment. It interacts with python in user-friendly manner.
- ogr/gdal: For reading, writing, and transforming geospatial data formats. This has ways to work with geospatial data, though fiona (see below) is nicer for reading and writing different geospatial formats.
- pyqgis: For anything and everything about GIS. This is the Python API for Quantum GIS. The user can work directly within QGIS via its intergrated Python console, or create standalone GIS apps.
- fiona: For making it easy to read/write geospatial data formats. It is for reading and writing GIS formats.
- matplotlib: For plotting needs. It does everything from scatterplots and histograms to choropleth maps to complex interactive visualizations.
- networkx: For working with networks. It is used for visualizing (integrates with matplotlib) and working with network data.
- pysal: For spatial econometrics needs (and more). This package covers everything from exploratory spatial data analysis (ESDA) right up to spatial econometric models.
- descartes: For plotting geometries in matplotlib. It is GeoJSON style data helper for matplotlib and shapely.
- geographiclib: For solving geodesic problems. It also converts between geographic, UTM, UPS, MGRS, geocentric, and local cartesian coordinates, and does geomagnetic field calculations.
- pyshp: For reading and writing shapefiles in pure Python.
- pyproj: For conversions between projections. This package provides an intuitive way of interacting with the Proj4 library for transforming data between coordinate reference systems.
- Seaborn: Python visualization library based on matplotlib. It provides a high-level interface for drawing attractive statistical graphics
- Bokeh: Python interactive visualization library that targets modern web browsers for presentation. Its goal is to provide elegant, concise construction of novel graphics in the style of D3.js, and to extend this capability with high-performance interactivity over very large or streaming datasets. 
- VisPy: Python library for interactive scientific visualization that is designed to be fast, scalable, and easy to use.


## Installation

### Setup
Go to this link : https://anaconda.org/anaconda/basemap. 

Find the code that install basemap package and execute it in command prompt. 

If you already have a Python environment set up, and you are using the conda package manager, you can get all packages by running

    conda install -c anaconda basemap=1.0.7

If the above method does not work, go to the same link and select ‘files’ tab. Then download tar.bz2 file that matches with your computer’s bit and python version. When the download is complete, put the files into your python directory.

Open the command prompt and type as follows;

    pip install <your tar.bz2 file name>

### Platform restriction - Any

### Dependent libraries 
(http://matplotlib.org/basemap/users/installing.html)

1. Requirements : matplotlib, numpy
2. Required libraries that ship with Basemap

    1) GEOS(Geometry Engine – Open Source) – Source code is included in the geos-3.3.3 directory. When building from source, it  must be built and installed separately from basemap.
    
    2) Cartographic Projections – Patched version automatically built into basemap.
    
3. Optional libraries : PIL(Python Imaging Library) is only needed for the following instance methods;

        bluemarble()  /  etopo()  /   shadedrelief()  /  warpimage()

## Examples : Please refer to the 'Examples' Folder

## Other interesting or useful features
- arcgisimage : connect ESRI (GIS mapping platform software company) server to download and plot the image file as background method

- nightshade : distinguish the day and night time of area by drawing dark regions on the map for night time. 

- barbs : plots wind barbs on the map 

- creating a basic map in 3D :

    1) With using Axes3D class and the method called add_collection3d, it is possible to add geographical data into 3D mapping.
    
    2) In Axes3D class, the method called bar3d draws 3D bars on 3D mapping.

## Summary and personal assessment of the library

After several steps of data arrangement, the basemap library allows us to make geographical mapping by transforming and plotting obtained longitude and latitude coordinates. As disadvantage, the basemap library requires the user to provide exact longitude and latitude coordinate in order to make correct globe projection. However, once the coordinates are known, the library is executed to draw actual 2D mapping including detailed boundaries of country and coastline, roads, and river based on datasets we provided. 
As a big advantage, the basemap library has linkage and accommodates with other essential libraries so that it can provide various functions that assist the reader to understand the main objective of the map. For instance, in our plotting home of the winner of the English Premier League, the reader can easily spot the winner’s home location in England by showing blue circle patch. In plotting the rate of endorsement of the President Barrack Obama, applying different color density enables the reader to capture the difference in the rate of endorsement for each state at once. Again, in our plotting earthquake at Haiti example, plotting point with red color helps the reader to figure out which area has high rate of phone call reporting during the earthquake at Haiti.
Consequently, the basemap library is very useful and powerful library in plotting 2D map and mandatory to whom tries to simplify the complex raw data into graphical representation for better interpretation.

## References
- Introduction — Basemap Matplotlib Toolkit 1.0.8 documentation. Matplotliborg. http://matplotlib.org/basemap/users/intro.html. (2.19.2017)

- Basemap tutorial — Basemap tutorial 0.1 documentation. http://basemaptutorial.readthedocs.io/en/latest/index.html, (2.19.2017)

- Anaconda Basemap download. https://anaconda.org/anaconda/basemap, (2.17.2017)

- European Soccer Kaggle Dataset. https://www.kaggle.com/hugomathien/soccer, (2.15.2017)

- McKinney, Wes. Python for data analysis: Data wrangling with Pandas, NumPy, and IPython. " O'Reilly Media, Inc.", 2012.

- Federal Election Commission Dataset. http://www.fec.gov/disclosurep/PDownload.do, (2.13.2017)

- Materials and IPython notebooks for "Python for Data Analysis" by Wes McKinney, published by O'Reilly Media. https://github.com/wesm/pydata-book, (2.13.2017)
