# Master of Maintenance

This is a repository for the Junction 2021 challenge by CGI/Kone. The notebook `exploration.ipynb` trains a LightGBM
model and tunes its hyper-parameters via Optuna. Before training the model, we combine the rarest categories in the
categorical features and optimize the threshold for each feature during the hyper-parameter optimization.