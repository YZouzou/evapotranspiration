# Part 3: ET0 Prediction

This section contains the notebooks used to split the data to train and test datasets, train the ML models, and explore the predictions and evaluation metrics.

## Directory definitions:
* **functions**: This directory contains the function and class definitions used in part 3.
* **algorithm_name (MLR, SVR, etc.)**: Directories named by algorithm names contain the trained models, predictions, evaluation metrics, and model parameters.
    * Note that if several sub-categories of a certain algorithm were tested, the algorithm, directory should contain sub directories for the sub-categories. Example: When using Support Vector Regression with several kernels we would have directories like `SVR/RBF` and `SVR/Polynomial`.

## Notebook definitions:
* **splitting_data**: The data is split to train and test datasets in this noteboook.
* **feature_combos**: The feature_combos.json file, which contains the feature combination definitions is generated in this notebook.
* **algorithm_name_models (Ex: MLR_models)**: Contains the code used to train the models of this algorithm.
* **performance_evaluation**: Contains an analysis and commentary on model results.