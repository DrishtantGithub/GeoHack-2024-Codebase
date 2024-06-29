# AMS 2013-2014 Solar Energy Prediction Contest

## Authors
- BoomerSooner
- StormMiner
- Will Cukierski

## Project Overview
This project worked on the Dataset available in the AMS 2013-2014 Solar Energy Prediction Contest, focusing on predictive modeling for renewable energy forecasting. The competition aimed to predict solar energy generation based on meteorological data from January 1, 1994, to December 31, 2007.

## Dataset
### Dataset Description
The dataset used in the contest includes:
- **GEFS Meteorological Data**: Covers variables such as temperature, precipitation, radiation, air pressure, humidity, and cloud cover. Data is provided in netCDF4 format, organized by ensemble members, time steps, and geographic coordinates.
- **Solar Energy Measurements**: Daily solar energy measurements (J m-2) collected from 98 Oklahoma Mesonet sites. Measurements were taken every 5 minutes and summed from sunrise to 23:55 UTC.

### Contents

1. **gefs_train.tar.gz** and **gefs_train.zip**:
   - Contains GEFS training data in netCDF4 format.
   - Each file holds grids for each ensemble member at every time step for specific variables.
   - Variables include:
     - apcp_sfc: 3-Hour accumulated precipitation at the surface (kg m-2)
     - dlwrf_sfc: Downward long-wave radiative flux average at the surface (W m-2)
     - dswrf_sfc: Downward short-wave radiative flux average at the surface (W m-2)
     - pres_msl: Air pressure at mean sea level (Pa)
     - pwat_eatm: Precipitable Water over the entire depth of the atmosphere (kg m-2)
     - spfh_2m: Specific Humidity at 2 m above ground (kg kg-1)
     - tcdc_eatm: Total cloud cover over the entire depth of the atmosphere (%)
     - tcolc_eatm: Total column-integrated condensate over the entire atmosphere (kg m-2)
     - tmax_2m: Maximum Temperature over the past 3 hours at 2 m above the ground (K)
     - tmin_2m: Minimum Temperature over the past 3 hours at 2 m above the ground (K)
     - tmp_2m: Current temperature at 2 m above the ground (K)
     - tmp_sfc: Temperature of the surface (K)
     - ulwrf_sfc: Upward long-wave radiation at the surface (W m-2)
     - ulwrf_tatm: Upward long-wave radiation at the top of the atmosphere (W m-2)
     - uswrf_sfc: Upward short-wave radiation at the surface (W m-2)

2. **train.csv**:
   - Total daily incoming solar energy (J m-2) measured at 98 Oklahoma Mesonet sites.
   - Measured by pyranometer every 5 minutes and summed from sunrise to 23:55 UTC.

3. **station_info.csv**:
   - Contains latitude, longitude, and elevation (m) of each Mesonet station.

4. **gefs_elevations.nc**:
   - NetCDF4 file with model elevations of GEFS grid points.
   - Includes elevation data for both control and perturbed runs.

## Additional Information

- The dataset provides comprehensive meteorological and solar energy data suitable for predictive modeling.
- For more details on file formats and reading methods, refer to the provided links and resources in the dataset description.
- Ensure to use elevations from **gefs_elevations.nc** for any elevation-based interpolation or modeling tasks.
- In our project to maintain the simplicity we have not used the gefs_elevation.nc data
  


## Institution
- American Meteorological Society (AMS)
- EarthRisk Technologies, Inc.

## Funding
The competition was sponsored by EarthRisk Technologies, Inc., providing prizes for top participants.

## References
- Kaggle Competition Page: [Link](https://www.kaggle.com/c/ams-2014-solar-energy-prediction-contest/overview)
