# FluShot

My solution for the Flu Shot Problem on DrivenData.org, where the goal is predict how likely individuals are to receive their H1N1 and seasonal flu vaccines, based on the National 2009 H1N1 Flu Survey.

I started out by performing an EDA into the structure and distributions of the predictors, and then also filtering predictors with high multicollinearity. I performed PCA on the numeric predictors and truncated SVD on the sparse 1 hot encoded categoricals, and combined the 2 to form the final dataset.

I then Applied Label Powerset to perform the multi-label prediction, and utilised CATBoost for which I tuned all the hyper-parameters.