# AutoML_examples
HHA 507 Assignment 9

 Dataset from Prof. Hans modified version of SPARCS - https://raw.githubusercontent.com/hantswilliams/HHA-507-2022/main/autoML/datasets/data_sparcs.csv) 

#### Two experiments: types of admissions
1. AutoML_1:
        - focused around binary classification sudying the type of admissions as the independent variables
        - The Xgboost was selected as the best model type as the metric value was 0.000298613, whereas the metric value for baseline model was 1.04705. Thus, the Xgboost performed better than the baseline model.
        - There were two values that equaled to 1, two values that equaled to 0.065 in the spearman correlations of models. The closer the AUC value is to 1, the more accurate the model is.
2. AutoML_2: total cost
        - focused around regression studying the total cost as the continuous variable
        - The Xgboost was selected as the best model type as the metric value was 0.000109814, whereas the metric value for baseline model was 0.00715457. Thus, the Xgboost performed better than the baseline model.
        - There were two values that equaled to 1, two values that equaled to 0.065 in the spearman correlations of models. The closer the AUC value is to 1, the more accurate the model is.
