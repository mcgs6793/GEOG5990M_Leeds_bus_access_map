# **GEOG5990M_Leeds_bus_access_map**

Analysis of bus service access in Leeds using bus stop and census data to create composite indices of supply and demand. Created for module GEOG5990M

**Aims and Project Background:**

This project aims to use open data to map bus service coverage in Leeds by creating and comparing composite indices of bus service supply and demand. Bus networks are a key element of public transport that help to reduce congestion and pollution and are a lifeline for some demographics such as younger and disabled people, or those with lower income(Le Vine and White, 2020). Despite this, rapid urban expansion and lack of awareness have led to inequalities in the distribution of urban transport networks which can make it harder for some of these bus-reliant groups to access employment, education and leisure facilities and cause social exclusion (Montero-Lamas et al., 2024). Considering this, this project intends to provide an overview of bus network coverage for transport planners in Leeds to help them better understand the gaps in the current network and identify areas for development.

**Data Used:**

The project is built on two main datasets: 

The first is bus stop data published by the West Yorkshire Combined Authority (West Yorkshire Combined Authority, 2019), which is downloadable in ESRI Shapefile format. This data includes point locations for bus stops in West Yorkshire up to 2019, with stop name and average hourly bus counts for peak and off-peak periods including 07:30-09:30, 12:00-14:00, 15:00 – 18:30 and 20:00 – 21:00.

The second main dataset is from the 2021 census available to download from the Office for National Statistics (2024). Variables related to demographics known to have a higher reliance on buses were downloaded via bulk download from the ONS, including tables: TS045, TS038, TS054, TS062, TS021, TS011, TS007 which cover age, disability, home ownership and ethnicity. These have been compiled into a single file called census.csv.

Alongside this data, Lower Super Output Area (LSOA) boundaries and population weighted centroids for each LSOA were downloaded through the government’s Open Geography Portal for use in creating the indices and mapping (ONS Geography, 2023; ONS Geography, 2024). 
All data is licensed under the Open Government Licence v3.0. https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/

**Running this Project and Requirements:**

The analysis is conducted in a Jupyter notebook called “bus_analysis.ipynb”, with all required data in the “Data” directory of this repository. The library requirements to run the notebook are shown in the table below with version information. You will also need to be able to run Jupyter notebooks on your device or have access to an online application to run them in the web browser, such as Google Colab.

**Library	Version Used**          
pandas	    2.2.3|
geopandas	  1.0.1|
matplotlib  3.9.2|
seaborn	    0.13.2|
scipy	     1.13.1|
numpy	     2.0.2|


*References*

Le Vine, S. and White, P. 2020. The shape of changing bus demand in England. Independent Transport Commission. [Online]. [Accessed 10/05/2025]. Available from: https://reesjeffreys.co.uk/wp-content/uploads/2020/01/ITC-Bus-market-in-England-Jan-2020.pdf

Montero-Lamas, Y., Fernández-Casal, R., Varela-García, F.-A., Orro, A. and Novales, M. 2024. A spatial statistical approach to estimate bus stop demand using GIS-processed data. Journal of Transport Geography. [Online]. 118, p103906. [Accessed 10/05/2025]. Available from: https://doi.org/https://doi.org/10.1016/j.jtrangeo.2024.103906 

Office for National Statistics. 2024. 2021 Census aggregate data. UK Data Service. [Online]. (30/04/2025). [Accessed 30/04/2025]. Available from: https://doi.org/DOI: https://dx.doi.org/10.5257/census/aggregate-2011-2 

ONS Geography. 2023. Lower layer Super Output Areas (December 2001) EW Population Weighted Centroids. [Online].  Office for National Statistics. [Accessed 30/04/2025]. Available from: https://geoportal.statistics.gov.uk/datasets/ons::lower-layer-super-output-areas-december-2001-ew-population-weighted-centroids/about

ONS Geography. 2024. Lower layer Super Output Areas (December 2021) Boundaries EW BFC (V10). [Online].  Office for National Statistics,. [Accessed 30/04/2025]. Available from: https://geoportal.statistics.gov.uk/datasets/ons::lower-layer-super-output-areas-december-2021-boundaries-ew-bfc-v10-2/about

West Yorkshire Combined Authority. 2019. West Yorkshire Bus Stops. [Online].  West Yorkshire Combined Authority. [Accessed 30/04/2025]. Available from: https://datamillnorth.org/dataset/vqxk4/west-yorkshire-bus-stops

