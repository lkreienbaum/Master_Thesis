# Master_Thesis of Louis Kreienbaum
In this Github account is the main code, I have used for my master thesis. 

The Data set used is from   Liu, H.; Su, M.; Lin, H.-X.; Wang, R.; Li, Y. ACS Omega 2022, 7, 18985-18996.

The inhibitor based features were calculated with the code of PropertyCalculator_Mordred.ipynb and are in the csv file HSP90_Mordred_Features.csv for the HSP90 features and HSP90_Kinase_Mordred.csv for the HSP90/p38 MAPK features. The protein-inhibitor complex based features were calculated using PropertyCalculator_PLIP.ipynb and saved in HSP90_PLIP_Features.csv . All notebooks uploaded contain the features from HSP90_Mordred_Features.csv. In order to obtain models for the kinase, or the protein-inhibitor complexes, change the csv file in 

A formatting issue, I have encountered from obtaining the csv-files from the property calculators, is the separation of rows in the csv-file. After calculating the properties, simply replace the "\n", which indicates the new row with \Enter. Also delete the apostrophes at the beginning and end. 

The code for the experimental and predicted values and feature importances of all models is RF_Model.ipynb. 

Using the inhibitor based features for HSP-90 the variance thresholding (fig. 3.3) and correlation variance thresholding (fig. 3.4, fig. 3.5) was applied using the code of RF_Correlation_Variance_Thresholding.ipynb. 

Furthermore, the feature selection scheme of fig. 3.6 was applied to the inhibitor based features (table 3.1) and the protein-ligand complex features (table 3.7, table 3.8, table 3.9) using the code of RF_Variance_&_Feature_Importance_Selection_(150,10).ipynb with alternating hyperparameters.

All hyperparameters were calculated with the code of RF_Hyperparameter_Optimization.ipynb (fig. 3.1, section 5.1).
