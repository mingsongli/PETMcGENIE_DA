# README for PETMcGENIE_DA Dataset

This README describes the contents and structure of the **PETMcGENIE_DA.nc** NetCDF file, which contains variables related to atmospheric and oceanic conditions during the Paleocene-Eocene Thermal Maximum (PETM). The dataset includes both mean values and variances for several important geochemical and environmental parameters.

## Variables

The file contains the following variables, each of which represents a different environmental parameter. Each variable has dimensions of `(lat=36, lon=36, t=2)` where `lat` represents latitude, `lon` represents longitude, and `t` represents time.

### Mean Variables:

1. **`atm_pCO2_Xa_mean`**:  
   Represents the **mean atmospheric CO2 concentration** during the PETM. This variable stores the average levels of atmospheric CO2, which plays a crucial role in understanding the greenhouse effect and climate change during the PETM.

2. **`ocn_sur_temp_Xa_mean`**:  
   Represents the **mean sea surface temperature (SST)**. This variable indicates the average temperature of the ocean's surface, which is critical for understanding global temperature changes during the PETM.

3. **`misc_pH_Xa_mean`**:  
   Represents the **mean ocean surface pH**. Ocean surface pH is essential for studying ocean acidification, which is closely related to the levels of CO2 dissolved in seawater.

4. **`sed_CaCO3_Xa_mean`**:  
   Represents the **mean calcium carbonate (CaCO3) content** in sediments. The presence of CaCO3 in marine sediments helps to understand carbon cycling and ocean chemistry changes during the PETM.

5. **`carb_sur_ohm_arg_Xa_mean`**:  
   Represents the **mean aragonite saturation state**. Aragonite is a form of calcium carbonate, and its saturation state in the ocean is critical for understanding the conditions necessary for the formation of certain marine organisms' skeletons and shells.

6. **`carb_sur_ohm_cal_Xa_mean`**:  
   Represents the **mean calcite saturation state**. Like aragonite, calcite is a form of calcium carbonate, and its saturation state is important for the formation of marine calcifying organisms.

### Variance Variables:

Each of the variables listed above also has a corresponding **variance** variable, which represents the variability of the measurements across different simulations or experiments:

- **`atm_pCO2_Xa_variance`**: Variance of atmospheric CO2 concentration.
- **`ocn_sur_temp_Xa_variance`**: Variance of sea surface temperature.
- **`misc_pH_Xa_variance`**: Variance of ocean surface pH.
- **`sed_CaCO3_Xa_variance`**: Variance of calcium carbonate content in sediments.
- **`carb_sur_ohm_arg_Xa_variance`**: Variance of aragonite saturation state.
- **`carb_sur_ohm_cal_Xa_variance`**: Variance of calcite saturation state.

## Time Dimension (`t`)

The dataset includes a time dimension `t` with two distinct time points, representing different periods relative to the PETM event:

- **t1**: This corresponds to the **pre-PETM** period. It represents the state of the environment before the onset of the Paleocene-Eocene Thermal Maximum.
- **t2**: This corresponds to the **PETM** period. It represents the state of the environment during the PETM, characterized by extreme global warming and ocean acidification.

## Coordinates

- **`Latitude (lat)`**: The latitude dimension consists of 36 grid points and is expressed in degrees.
- **`Longitude (lon)`**: The longitude dimension consists of 36 grid points and is expressed in degrees.

## Supporting Information

This dataset supports the findings presented in **Li et al., 2024 Nature Geoscience**. The study investigates the dramatic shifts in ocean chemistry during the Paleocene-Eocene Thermal Maximum (PETM), a rapid climate event 56 million years ago marked by extensive carbon release and ocean acidification. The dataset is instrumental in understanding the geochemical and environmental changes during this period.

## Scripts for Generating This Dataset

The scripts used to generate this dataset are available as part of the following Zenodo repository:

**Citation:**

Mingsong Li. (2024). *mingsongli/deepDA: v1.0.0 - Li et al., 2024 Nature Geoscience Release (v1.0.0)*. Zenodo. [https://doi.org/10.5281/zenodo.13777776](https://doi.org/10.5281/zenodo.13777776)
