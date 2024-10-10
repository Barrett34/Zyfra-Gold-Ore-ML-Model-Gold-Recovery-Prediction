# Zyfra-Gold-Ore-ML-Model-Gold-Recovery-Prediction
Zyfra is a gold ore company that is in need of a machine learning model to predict how much gold can be recovered from a gold ore.

## Introduction: 

In this project, we are creating a machine learning model for the company Zyfra. The company creates efficient solutions for heavy industry. The model will predict how much gold can be recovered from a gold ore. The model's goal is to aid the optimization of production and the elimination of unprofitable parameters.

## Datasets
- gold_recovery_train.csv
- gold_recovery_test.csv
- gold_recovery_full.csv

## Conclusion
The project's goal of creating a prototype of a machine learning model that can predict the recovery rate of gold from gold ore has been met. The data was processed and analyzed during the project, and a random forest model was built and trained as a result. The final model outperforms the constant model: the trained model's error is 7.7%, while the constant model's error is 7.9%. During the project, the following steps were taken:

- read and analyzed the data (prepared an EDA report for each dataset)
- data that has been pre-processed (processing missing values, replacing data type, checking for duplicates)
- double-checked the enrichment efficiency calculation.
- investigated how metal concentrations (Au, Ag, Pb) change during the purification process. We can conclude that the concentration of each metal varies  depending on the stage of purification: gold concentration gradually increases with each stage, silver concentration decreases, and lead concentration increases in the first three stages.
- performed a granule size analysis on the training and test sets to ensure that the granule sizes are roughly evenly distributed in the training and test sets.
- examined the total concentration of all metals at various stages, identifying and removing anomalies (a large number of zeros) from all datasets.
- created functions to compute sMAPE and final sMAPE
- compared the performance of various models (DecisionTreeRegressor (), RandomForestRegressor, LinearRegression) and how the best random forest model was selected using the hyperparameters n estimators = 15 and max depth = 4. The final model's work was tested on a test sample, and it performed well: the trained model's error is 7.7%, while the constant error is 7.9%.
