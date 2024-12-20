# LSTM static attribute sensativity analysis for ungauged basin performance in a heterogeneous modeling framework

## Analysis notebook
The main analysis for this experiment is done with the notebook: `attribute_PCA_visualization.ipynb`.

## Lumped hydrofabric generation
This code has two main sections.  
Section 1: Getting appropriate CAMELS shapefile data and basin lists to extract the correct basins  
Section 2: Plotting the CAMELS catchments vs the Hydrofabric lumped basins to see how they compare

##  Hydrofabric Hydroatlas Sampling
This code has three main sections
Section 1: Sample every hydroatlas attribute for each hydrofabric
Section 2: Sample the hydroatlas attributes at the centroid of the CAMELS basins
Section 3: Generate a PCA of the hydroatlas attributes sampled within the CAMELS basins  

## Data
Data for running the notebooks can be found at https://zenodo.org/records/14532711. These data include run files from NeuralHydrology. To run the notebook, the data should be downloaded from Zenodo, then a little bit of unpacking and manipulation to the file paths is needed.
A local directory should be created with the name `LSTM_for_NextGen_results`, and the downloaded data from Zenodo should be unpacked in that directory. For final results, the zip files to unpack are `LSTM_for_NextGen_attributes_results_7_ensembles` and `PC_10_20_50_100_200_ensembles.zip`. Other zip files in the Zenodo directory have individual model runs, and means from smaller ensembles. Not that while the following data sets are loaded in the notebook, they are not used in the analysis and figures: nonEnsemble, ensemble5 and ensembles6. These can be removed from the notebook, if the user desires. 

### Individual runs
The published results rely on an ensemble mean for the LSTM results, to avoid the uncertainty that comes from random initializations during training. We also in Zenodo is a zip file called `individual_runs.zip` which has all the simulation data, including the individual runs. This file is much larger than the ensemble means, and isn't needed to run the notebook.