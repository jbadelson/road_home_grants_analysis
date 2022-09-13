# Road Home Grants Analysis
An analysis of Road Home grants

Shapefile and processed file directories can be found on Google Drive

I did not include a requirements.txt file because I ran into some problems with conflicting dependencies in Conda and didn't want to cause any headaches on the install. I believe installing GeoPandas and Seaborn will install all packages needed to run the notebook and will avoid any conflicts.

The rh_analysis.ipynb file is the version of the analysis discussed during the Zoom call on 9/9/2022. This analysis includes all blocks, not just those with more than 3 feet of flooding.

Processing of the files has been separated out into its own file (1-processing.ipynb) which DOES filter the blocks to only include those where a minimum of 3 feet of flooding was reported. That notebook requires the shapefiles from the Google Drive and will generate CSV and GeoJSON files for analysis. Files with flood_GT3 in their name only include Road Home data for blocks with greater than 3 feet of flooding. Demographic data is included for all blocks and neighborhoods, regardless of flooding. 

The same exploratory analysis was rerun on the the flood_GT3 files and can be found in 2-exploratory_analysis.ipynb. Some markdown cells have been excluded since the statistics they reference do not reflect the results when using the flood_GT3 files.
