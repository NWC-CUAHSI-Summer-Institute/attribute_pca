# LSTM info for attributes sensitivity experiment
The LSTM used in this experiment was trained with NeuralHydrology (Kratzert et al., 2022). The main unique data source for this experiment comes in the form of static attributes, which are used to help the LSTM model generalize to new locations. The results in the paper come from test basins that were not included in the training set, meaning that the results are out-of-sample in space. 

## config_files
This directory contains the configuration files that were used to train and evaluate the LSTM models.

## basin_lists
This directory contains lists of basins that were used in the model training and model testing. The published results come from the basins in the testing set, not from the training set.

## scripts
This directory contains shell scripts that were used to train the LSTM models, to run the ensemble means and to run the evaluation. Note that all of the calculations are done with NeuralHydrology, these scripts are just tools to run the utilities of NeuralHydrology.

Kratzert, F., Gauch, M., Nearing, G., & Klotz, D. (2022). NeuralHydrology---A Python library for Deep Learning research in hydrology. Journal of Open Source Software, 7(71), 4050.