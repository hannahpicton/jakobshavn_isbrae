# Jakobshavn Isbrae 
This repository is associated with the manuscript ‘A reassessment of the role of atmospheric and oceanic forcing on ice dynamics at Jakobshavn Isbræ (Sermeq Kujalleq), Ilulissat Icefjord’, submitted to the Journal of Geophysical Research: Earth Surface. In this study, we use satellite imagery and remotely-sensed datasets to extend observations of ice dynamics at Jakobshavn Isbræ between 2018 and 2023. We provide timeseries of key glaciological parameters, analysing variability in ice surface velocity, ice surface elevation, ice discharge, terminus position, and rigid mélange extent. We then use a combination of hydrographic data obtained from conductivity-temperature-depth (CTD) sensors, surface air temperature data measured at a local weather station, and modelled estimates of surface runoff, to explore the potential influence of oceanic and atmospheric forcing on ice dynamics at Jakobshavn Isbræ over this most recent five-year period. 

## Ice Surface Velocity 
A timeseries of ice velocity was extracted across Jakobshavn Isbrae using NASA’s MEaSUREs Inter-mission Time Series of Land Ice Velocity and Elevation (ITS_LIVE) product (https://its-live.jpl.nasa.gov/), accessed using the cloud-optimized Zarr datacubes. All available 6-day and 12-day image-pair velocities were downloaded between 01/01/2018 and 31/12/2022, before being sampled at 5km intervals along the centreline of Jakobshavn Isbræ (T, T5, T10, T15, T20, T30).  

## Ice Surface Elevation 
Ice elevation was assessed using a gridded dataset (https://doi.org/10.5067/ATLAS/ATL15.003) derived from the ATLAS/ICESat-2 L3B Slope-Corrected Land Ice Height Time Series product (https://doi.org/10.5067/ATLAS/ATL11.004). The gridded product (ATL15) provides estimates of elevation change relative to 01/01/2020 at 3-monthly intervals. The dataset was downloaded at a resolution of 1KM, with the elevation change ('delta_h') extracted at each of the sampling locations described above (T, T5, T10, T15, T20, T30). 

## Ice Discharge 
A timeseries of solid ice discharge from Jakobshavn Isbrae was extracted from Mankoff et al. (2020), provided on the GEUS dataverse (https://doi.org/10.22008/promice/data/ice_discharge/d/v02). This dataset provides estimates of ice discharge through algorithmically generated gates positioned ~ 5 km upstream from the baseline terminus of all fast-flowing ice (>100 m/yr).

## Terminus Position
Terminus positions derived between 2018 and 2022 were downloaded from the MEaSUREs Weekly to Monthly Greenland Outlet Glacier Terminus Positions from Sentinel-1 Mosaics (2018-2022; https://nsidc.org/data/nsidc-0781/versions/1), whilst terminus positions derived between 2022 and 2023 were manually digitised from SAR imagery (https://doi.org/10.5067/WXQ366CP8YDE). Terminus position change was conducted using MaQiT (https://liverpoolgee.wordpress.com/maqit/), with the the curvilinear box method being employed. 

## Rigid Mélange Extent
The maximum extent of rigid mélange was measured at a monthly resolution, relative to the contemporaneous terminus position. The frontal position of the mélange was manually digitised from continuous ITS_LIVE 6-day (2018-2022) and 12-day (2022-2023) velocity pairs; this method assumes that a coherent velocity signal over the mélange is indicative of rigidity, as outlined by Chudley et al. (2023; https://doi.org/10.1038/s41467-023-37764-7).

