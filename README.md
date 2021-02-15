# CCN-proxy-modeling

## Project description

We are working on a project to model atmospheric cloud condensation nuclei proxy concentrations, specifically n100 proxy concentrations. The n100 proxy concentration data was provided to us internally by [INAR](https://www.helsinki.fi/en/inar-institute-for-atmospheric-and-earth-system-research) and can be found in the [here](/data/N100_proxy/). A list of the stations and corresponding metadata can be found [here](/metadata/measurement_sites_info.txt). The training data for our models contains modified Copernicus Atmosphere Monitoring Service Information (CAMS, 2021). Neither the European Commission nor ECMWF is responsible for any use that may be made of the information it contains. The individual CAMS reanalysis data sets can be found in the [data folder](/data/) of this repository. The same repository also contains a file with the [fully merged dataset](/data/full_data.csv) used for model training. A list of the variables included in the datasets can be found [here](/metadata/variable_names.txt).

This folder contains multiple Jupyter notebooks. The individual datasets mentioned above are pre-processed and merged in the [data pre-processing notebook](data%20pre-processing.ipynb). The exploratory data analysis with visualizations of the input data can be found in the [exploratory data analysis notebook](exploratory%20data%20analysis.ipynb). Lastly, there are two notebooks containing models. The [modelling notebook](modelling.ipynb) contains Linear Regression and Random Forest Regression models for predicting n100 proxy concentrations. The [xgboost notebook](xgboost.ipynb) contains an XGBoost regressor model.


## XGBoost 

### Dependencies

Regressor
```
conda install -c conda-forge xgboost
```

Graph 
```
conda install -c conda-forge graphviz xorg-libxrender xorg-libxpm python-graphviz
```
