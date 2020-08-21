## Linear Regression 
### Best fit data preparation - 
1) Linear assumption: Assume the data is linear and will give best prediction.
2) Remove collinearity: Means lines are modeled by the same line. Remove this. 
3) Gaussian (normal) distribution
4) Rescale data: Normalize it for normal distribution.
5) Remove noise: Remove Outliers 

### Best error function/cost factor - _RMSE_

**Left to read - How to remove collinearity and outliers to remove noise.**

- _Two types of algorithms- Parametric & Non-parametric_

## Classical ML vs Deep Learning
### Deep learning advantages:

1) Suitable for high complexity problems
2) Better accuracy, compared to classical ML
3) Better support for big data
4) Complex features can be learned

### Deep learning disadvantages:

1) Difficult to explain trained data
2) Require significant computational power

### Classical ML advantages:

1) More suitable for small data
2) Easier to interpret outcomes
3) Cheaper to perform
4) Can run on low-end machines
5) Does not require large computational power

### Classical ML disadvantages:

1) Difficult to learn large datasets
2) Require feature engineering
3) Difficult to learn complex functions

![](https://video.udacity-data.com/topher/2020/May/5ebed4d4_aws-mle-ml-stack-v3/aws-mle-ml-stack-v3.jpg)

#### Bias
Error that results from inaccurate assumptions in model training (that are made to simplify the training process). Bias measures how inaccurate the model prediction is in comparison with the true output. It is due to erroneous assumptions made in the machine learning process to simplify the model and make the target function easier to learn. High model complexity tends to have a low bias.

#### Variance 
Variance measures how much the target function will change if different training data is used. Variance can be caused by modeling the random noise in the training data. High model complexity tends to have a high variance.

```
As a general trend, parametric and linear algorithms often have high bias and low variance, whereas non-parametric and non-linear algorithms often have low bias and high variance. Low bias means fewer assumptions about the target function. Some examples of algorithms with low bias are KNN and decision trees. 
Having fewer assumptions can help generalize relevant relations between features and target outputs. 
In contrast, high bias means more assumptions about the target function. Linear regression would be a good example (e.g., it assumes a linear relationship). Having more assumptions can potentially miss important relations between features and outputs and cause underfitting.

Low variance indicates changes in training data would result in similar target functions. For example, linear regression usually has a low variance. High variance indicates changes in training data would result in very different target functions. 
For example, support vector machines usually have a high variance. High variance suggests that the algorithm learns the random noise instead of the output and causes overfitting.

Generally, increasing model complexity would decrease bias error since the model has more capacity to learn from the training data. But the variance error would increase if the model complexity increases, as the model may begin to learn from noise in the training data.

The goal of training machine learning models is to achieve low bias and low variance. The optimal model complexity is where bias error crosses with variance error.
```  

#### Overfitting
Overfitting refers to the situation in which models fit the training data very well, but fail to generalize to new data.

#### Underfitting
Underfitting refers to the situation in which models neither fit the training data nor generalize to new data.
