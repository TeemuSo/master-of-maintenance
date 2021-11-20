# Master of Maintenance

This is a repository for the Junction 2021 challenge by CGI/Kone. The repository contains two notebooks.
## `binary_model.ipynb`
The notebook trains a model that predicts whether a technician should be dispatched to the equipment based on the given
input. We train a LightGBM model and tune its hyper-parameters via Optuna. Before training the model, we combine
the rarest categories in the categorical features and optimize the threshold for each feature during the hyper-parameter optimization.

## `closes_claims.ipynb`
The notebook is used for finding similar maintenanse cases to the wanted test case. This notebook uses ipywidgets to create user interface, which utilizes K-NearestNeighbors (K-NN) search with K=5. The K-NN is trained on only valid claims. If the user does not want to search for test case manually, he can "Take random case" from test set. The test set consists of cases where action predictions were false.