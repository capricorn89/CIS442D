# Basemap Tutorial

## Motivation
TheBasemap toolkit (URL: http://matplotlib.github.com/basemap/ ), an add-on to matplotlib, enables plotting 2D data on maps in Python. 
The main objective of basemap toolkit is to provide globe projections by transforming projecting latitude and longitude coordinates on the globe onto a two-dimensional Matplotlib plot. 
Contours, images, vectors, lines, or points can be plotted in Matplotlib, which is then used to display roads, shoreline, river, coastline, or any kinds of boundary datasets from various generic mapping tools such as ArcGIS mapping programming.
Therefore, the basemap library can give desired map projection region in user-friendly manner. 
This 2D map projection feature can satisfy various needs, such as climate and weather forecasting, future earthquake research, oil and gas detection, or any subject area that requires detailed observation of globe with high accuracy as well as clear readability of projected map region produced by the basemap.


## Context


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

### Dependent libraries (http://matplotlib.org/basemap/users/installing.html)
1. Requirements : matplotlib, numpy
2. Required libraries that ship with Basemap

    1) GEOS(Geometry Engine – Open Source) – Source code is included in the geos-3.3.3 directory. When building from source, it  must be built and installed separately from basemap.
    
    2) Cartographic Projections – Patched version automatically built into basemap.
    
3. Optional libraries : PIL(Python Imaging Library) is only needed for 

        bluemarble() ‘etopo()’, ‘shadedrelief()’ and ‘warpimage()’ 
        
 instance methods.

