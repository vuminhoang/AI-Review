# Overfitting versus Underfitting problem
## 1. Understanding Bias and Varriance
In machine learning, bias and variance are key concepts that influence a model's ability to generalize.
They describe errors introduced by the model assumptions and data sensitivity:

### Bias
Bias can be thought of as the error between the average model prediction and the ground truth.

Higher bias → Worse model performance!

### Varriance
Variance refers to changes in the model when using different portions of the training data set.

Higher variance means that the model is too sensitive to the training data, capturing noise as if it were a true pattern, which leads to overfitting.

### Over/Under fitting
| **Characteristic**       | **Overfitting**                             | **Underfitting**                          |
|---------------------------|---------------------------------------------|-------------------------------------------|
| **Model Complexity**      | Too complex                                | Too simple                                |
| **Performance**           | Good on training data, bad on test data   | Bad on both training and test data       |
| **Causes**                | Sensitive to noise, overly fits training data | Fails to capture data trends             |
| **Bias&Variance**        | Low Bias, High Variance       | High Bias, Low Variance      |

## 2. Visualizing Overfitting and Underfitting. 

