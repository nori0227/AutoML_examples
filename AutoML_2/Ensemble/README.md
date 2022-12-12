# Summary of Ensemble

[<< Go back](../README.md)


## Ensemble structure
| Model             |   Weight |
|:------------------|---------:|
| 3_Default_Xgboost |        1 |

## Metric details
|           |       score |     threshold |
|:----------|------------:|--------------:|
| logloss   | 0.000109814 | nan           |
| auc       | 1           | nan           |
| f1        | 0.133333    |   0.000187796 |
| accuracy  | 0.988405    |   0.000187796 |
| precision | 0.0714286   |   0.000187796 |
| recall    | 1           |   2.82334e-05 |
| mcc       | 0.265706    |   0.000187796 |


## Metric details with threshold from accuracy metric
|           |       score |     threshold |
|:----------|------------:|--------------:|
| logloss   | 0.000109814 | nan           |
| auc       | 1           | nan           |
| f1        | 0.133333    |   0.000187796 |
| accuracy  | 0.988405    |   0.000187796 |
| precision | 0.0714286   |   0.000187796 |
| recall    | 1           |   0.000187796 |
| mcc       | 0.265706    |   0.000187796 |


## Confusion matrix (at threshold=0.000188)
|                  |   Predicted as long |   Predicted as short |
|:-----------------|--------------------:|---------------------:|
| Labeled as long  |                5536 |                   65 |
| Labeled as short |                   0 |                    5 |

## Learning curves
![Learning curves](learning_curves.png)
## Confusion Matrix

![Confusion Matrix](confusion_matrix.png)


## Normalized Confusion Matrix

![Normalized Confusion Matrix](confusion_matrix_normalized.png)


## ROC Curve

![ROC Curve](roc_curve.png)


## Kolmogorov-Smirnov Statistic

![Kolmogorov-Smirnov Statistic](ks_statistic.png)


## Precision-Recall Curve

![Precision-Recall Curve](precision_recall_curve.png)


## Calibration Curve

![Calibration Curve](calibration_curve_curve.png)


## Cumulative Gains Curve

![Cumulative Gains Curve](cumulative_gains_curve.png)


## Lift Curve

![Lift Curve](lift_curve.png)



[<< Go back](../README.md)
