# Summary of 2_DecisionTree

[<< Go back](../README.md)


## Decision Tree
- **n_jobs**: -1
- **criterion**: gini
- **max_depth**: 3
- **num_class**: 6
- **explain_level**: 2

## Validation
 - **validation_type**: split
 - **train_ratio**: 0.75
 - **shuffle**: True
 - **stratify**: True

## Optimized metric
logloss

## Training time

25.8 seconds

### Metric details
|           |   Elective |   Emergency |   Newborn |   Not Available |   Trauma |     Urgent |   accuracy |   macro avg |   weighted avg |   logloss |
|:----------|-----------:|------------:|----------:|----------------:|---------:|-----------:|-----------:|------------:|---------------:|----------:|
| precision |          1 |           1 |         1 |               0 |        0 |   0.950581 |   0.996157 |    0.65843  |       0.992505 | 0.0176364 |
| recall    |          1 |           1 |         1 |               0 |        0 |   1        |   0.996157 |    0.666667 |       0.996157 | 0.0176364 |
| f1-score  |          1 |           1 |         1 |               0 |        0 |   0.974665 |   0.996157 |    0.662444 |       0.994285 | 0.0176364 |
| support   |        845 |        2807 |       428 |               5 |       12 | 327        |   0.996157 | 4424        |    4424        | 0.0176364 |


## Confusion matrix
|                          |   Predicted as Elective |   Predicted as Emergency |   Predicted as Newborn |   Predicted as Not Available |   Predicted as Trauma |   Predicted as Urgent |
|:-------------------------|------------------------:|-------------------------:|-----------------------:|-----------------------------:|----------------------:|----------------------:|
| Labeled as Elective      |                     845 |                        0 |                      0 |                            0 |                     0 |                     0 |
| Labeled as Emergency     |                       0 |                     2807 |                      0 |                            0 |                     0 |                     0 |
| Labeled as Newborn       |                       0 |                        0 |                    428 |                            0 |                     0 |                     0 |
| Labeled as Not Available |                       0 |                        0 |                      0 |                            0 |                     0 |                     5 |
| Labeled as Trauma        |                       0 |                        0 |                      0 |                            0 |                     0 |                    12 |
| Labeled as Urgent        |                       0 |                        0 |                      0 |                            0 |                     0 |                   327 |

## Learning curves
![Learning curves](learning_curves.png)

## Decision Tree 

### Tree #1
![Tree 1](learner_fold_0_tree.svg)

### Rules

if (Type of Admission > 0.5) and (Type of Admission <= 1.5) then class: Emergency (proba: 100.0%) | based on 8,419 samples

if (Type of Admission <= 0.5) then class: Elective (proba: 100.0%) | based on 2,536 samples

if (Type of Admission > 0.5) and (Type of Admission > 1.5) and (Type of Admission <= 2.5) then class: Newborn (proba: 100.0%) | based on 1,286 samples

if (Type of Admission > 0.5) and (Type of Admission > 1.5) and (Type of Admission > 2.5) then class: Urgent (proba: 95.15%) | based on 1,030 samples





## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)
## Confusion Matrix

![Confusion Matrix](confusion_matrix.png)


## Normalized Confusion Matrix

![Normalized Confusion Matrix](confusion_matrix_normalized.png)


## ROC Curve

![ROC Curve](roc_curve.png)


## Precision Recall Curve

![Precision Recall Curve](precision_recall_curve.png)



## SHAP Importance
![SHAP Importance](shap_importance.png)

## SHAP Dependence plots

### Dependence Elective (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_Elective.png)
### Dependence Emergency (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_Emergency.png)
### Dependence Newborn (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_Newborn.png)
### Dependence Not Available (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_Not Available.png)
### Dependence Trauma (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_Trauma.png)
### Dependence Urgent (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_Urgent.png)

## SHAP Decision plots

### Worst decisions for selected sample 1 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_0_worst_decisions.png)
### Worst decisions for selected sample 2 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_1_worst_decisions.png)
### Worst decisions for selected sample 3 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_2_worst_decisions.png)
### Worst decisions for selected sample 4 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_3_worst_decisions.png)
### Best decisions for selected sample 1 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_0_best_decisions.png)
### Best decisions for selected sample 2 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_1_best_decisions.png)
### Best decisions for selected sample 3 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_2_best_decisions.png)
### Best decisions for selected sample 4 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_3_best_decisions.png)

[<< Go back](../README.md)
