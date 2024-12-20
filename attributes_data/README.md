# CAMELS Static Attributes with Extention of NOAH-MP and HydroAtlas
This directory contains static attributes for the CAMELS basins (Addor et al., 2017), with additional attributes coming NOAH-MP and HydroAtlas.

## Data structure
The data from HydroAtlas and NOAH-MP were formatted to conform with the existing CAMELS attributs, and they are located in these files:
 - `camels_attributes_v2.0/camels_hydroatlas.txt`: This file contains HydroAtlas static attributes Summarized over the CAMELS basins.
 - `camels_attributes_v2.0/camels_hydroatlas_pca.txt`: This file contains a dimensional reduction of the HydroAtlas static attributes Summarized over the CAMELS basins.
 - `camels_attributes_v2.0/camels_noahmp.txt`: This file contains parameters from NOAH-MP summarized over the CAMELS basins.
There is redundant data in these two directories: `NOAH_MP` and `hydroATLAS_Camels`, but for ease of use in NeuralHydrology with the existing CAMELSUS data loader, it is best to use the data listed above from `camels_attributes_v2`.

## References
Addor, N., Newman, A. J., Mizukami, N., and Clark, M. P.: The CAMELS data set: catchment attributes and meteorology for large-sample studies, Hydrol. Earth Syst. Sci., 21, 5293–5313, https://doi.org/10.5194/hess-21-5293-2017, 2017.
