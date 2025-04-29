# Introduction

This `Obesity Level` data set is survey data to model weight class from South American countries along with simuklated responses to add to the observation count. A classification task will be fit with multiple different models in order to determine the best fit.

# Data Set

## Response Variable

The response variable, weight class (also referred to as "obesity level") originally contains 7 classes. They are the following:

* Underweight
* Normal Weight
* Overweight I
* Overweight II
* Obese I
* Obese II
* Obese III

It is unclear the exact BMI specifications that distinguish one group from another.

## Potential Predictors

The potential predictors are below:

* Gender
* Age
* Height
* Weight
* Do you have a family history of higher weight?
* Do you eat high calorie food regularly?
* Are there vegetables in your meals regularly?
* How many meals per day usually?
* Do you eat between meals?
* Do you smoke?
* How much water do you drink daily (in levels/categories)?
* Do you monitor caloric intake?
* How many days do you exercise a week (in levels/categories)?
* How many hours a day are spent using technology (in levels/categories)?
* How often do you drink alcohol (in levels/categories)?
* What type of transportation do you use most?
* What is your weight level?

Variable selection is discussed in the `Weight_modeling.rmd` file above.

# Models

Various models were fit in order to determine the overall best model fit. These include...

* kNN
* Logistic
* Local Logistic (**gamLoess**)
* Simple CART
* Ensemble CART
* SVM

These models are all trained on a training set in order to fix hyperparameter values and then tested on the test set for overall comparison using Log Loss and Accuracy as metrics for this analysis and model selection.
