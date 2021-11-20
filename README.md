# Master of Maintenance

This is a repository for the Junction 2021 challenge by CGI/Kone. The repository contains two notebooks.
## `binary_model.ipynb`
The notebook trains a model that predicts whether a technician should be dispatched to the equipment based on the given
input. We train a LightGBM model and tune its hyper-parameters via Optuna. Before training the model, we combine
the rarest categories in the categorical features and optimize the threshold for each feature during the hyper-parameter optimization.