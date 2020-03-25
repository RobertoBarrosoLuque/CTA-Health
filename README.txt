Documentation for CAPP-30122 Project
Roberto Barroso, Hana Passen, Charmaine Runes

Python Version: 
    3.6+

External libraries: Please run the following commands, in order: 
-python3.7 -m venv env
-source env/bin/activate
-sudo pip install --upgrade pip
-sudo apt-get install libgeos++-dev
-sudo apt-get install libproj-dev
-sudo apt install python3-rtree
-sudo pip3.7 install -r requirements.txt 

To Run the Software: in terminal, run: 
- python draft_ui.py

Python Libraries: pandas, numpy, geopandas, shapely, matplotlib, bs4.

Files: 
    - requirements.txt: a txt file containing the requirements for the virtual
                        environment
    - cta_classes.py: a module containing the methods for constructing MetroLine
                      and MetroStop classes, generating shapefiles for each 
                      MetroLine, and plotting the lines
    - cta_data_wrangle.py: a module containing the functions to request CTA stop
                           data through an API, and process that data
    - line_scraper.py: a module for webscraping CTA line data for the ordered
                       list of stops
    - health_wrangle.py: a module for collecting City of Chicago public health
                         indicator data from the City Health Portal API, and 
                         cleaning that data
    - census_data_wrangle.py: a module for loading and cleaning a CSV with the
                              demographic data for each census tract downloaded
                              from the census website
    - acs_ph_combine.py: a module that merges the public health and demographic
                         dataframes, and uses indicators from each to calculate
                         an aggregated health score, and an adversity index for
                         each census tract

Directories: 
    - ui: a directory containing the user interface files
    - data: a directory containing all the data files we have used
 
