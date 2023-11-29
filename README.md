# Jakobshavn Isbrae 

## Terminus Position 
The 'terminus_position_MaQiT' folder contains the terminus position shapefiles for Jakobshavn Isbrae (2018-2023). Terminus positions were manually digitised between 2022 and 2023 from SAR imagery, for the purposes of this study. Those provided between 2018 and 2022 were downloaded from the MEaSUREs Weekly to Monthly Greenland Outlet Glacier Terminus Positions from Sentinel-1 Mosaics (2018-2022; https://nsidc.org/data/nsidc-0781/versions/1). 

Terminus position change analysis was conducted using MaQiT (https://liverpoolgee.wordpress.com/maqit/), with the curvilinear box method being employed. The centreline shapefile used and the MaQiT output CSV are both provided within the 'terminus_position_MaQiT' folder. The script 'terminus_position' uses this output CSV file to plot a graph of terminus position change over the study period. 

## Ice Velocity 
A timeseries of ice velocity was extracted across Jakobshavn Isbrae using NASA’s MEaSUREs Inter-mission Time Series of Land Ice Velocity and Elevation (ITS_LIVE) product (https://its-live.jpl.nasa.gov/), accessed using the cloud-optimized Zarr datacubes. The script 'ice_velocity_download' downloads all available 6-day and 12-day image-pair velocities within the Jakobshavn region between 01/01/2018 and 31/12/2022. The script 'ice_velocity_sample' then extracts velocity at sampling locations positioned on the centreline of Jakobshavn Isbrae (T, T5, T10, T15, T20, T30), exporting the data to a CSV. The script 'ice_velocity_plot' then uses this CSV to plot a graph showing the ice velocity at each sampling location over the study period. 

## Surface Runoff
The 'surface_runoff' script uses Version 5 of the 'Streams, Outlets, Basins, and Discharge [k=1.0]' dataset (Mankoff et al., 2020) provided on the GEUS dataverse (https://doi.org/10.22008/FK2/XKQVL7). It should be noted that as Jakobshavn Isbrae is a marine-terminating glacier, only the 'ice' datasets are downloaded (the 'land' files are not needed). The script uses both MAR and RACMO data, plotting graphs of daily discharge and annual cumulative discharge across the primary hydrological basin of Jakobshavn Isbrae between 2018 and 2023. 

## Ice Discharge 

## Rigid Mélange Extent 
