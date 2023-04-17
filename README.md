# Analysis of California's 2021 Congressional Districts Using Gerrychain

This project aims to analyze and compare different redistricting plans for the state of California using the GerryChain algorithm. It consists of several Jupyter Notebooks and Python scripts to process and visualize the data.

## Table of Contents

1. [Results](#results)
2. [Getting Started](#getting-started)
3. [Project Structure](#project-structure)
4. [Data Sources](#data-sources)

## Results



## Getting Started

To set up the project, follow these steps:

1. Clone the repository.
2. Create a Conda environment using the provided `conda-environment.yml` file:

```conda env create -f conda-environment.yml```

3. Activate the environment:

```conda activate gerrychain```

4. Run the Jupyter Notebooks in order to process the data and visualize the results.

## Project Structure

The project is structured as follows:

- `notebooks/` - Contains Jupyter Notebooks for various stages of the project:
- `data-preparation.ipynb` -- Fetches required data from the internet and cleans it.
- `connect-islands.ipynb` - Processes the raw data and connects islands in the map.
- `run-gerrychain.ipynb` - Runs the GerryChain algorithm on the processed data and creates visualizations.
- `conda-environment.yml` - Conda environment file with the required dependencies for the project.
- `README.md` - This file.

## Data Sources
* Alarm_Redist (2023). Alarm_Redist 2020 Congressional Districts.
Retrieved from https://raw.githubusercontent.com/alarm-redist/census-2020/main/census-vest-2020/ca_2020_block.csv
  * "To produce election data using 2020 precinct boundaries, election results were projected down to the 2010 block level using voting-age population as weights. Results for 2020 blocks were then estimated using 2010 blocks and the land-use-based crosswalk files from VEST. Finally, 2020 blocks were aggregated to 2020 Census VTDs using the Census' 2020 block assignment files."
  * Provides a ready-to-use dataset for tying in 2020 election results with the 2020 census blocks.

* U.S. Census Bureau. (2023). TIGER/Line Shapefiles for 2020 Census Block Groups. Retrieved from https://www2.census.gov/geo/tiger/TIGER2020/TABBLOCK20/tl_2020_06_tabblock20.zip
  * 2020 shapfiles for California.

* U.S. Census Bureau. (2023). Block Assignment Files for California, 2020 Census. Retrieved from https://www2.census.gov/geo/docs/maps-data/data/baf2020/BlockAssign_ST06_CA.zip
  * Connects 2010 congressional districts with 2020 blocks.

* California Citizens Redistricting Commission. (2023). Final Congressional Districts Equivalency File for the 2020 Census. Retrieved from https://wedrawthelines.ca.gov/wp-content/uploads/sites/64/2023/01/CD-Final-equiv.xlsx?emrc=63dc56ef11a47
  * Connects 2021 congressional districts with 2020 blocks.
