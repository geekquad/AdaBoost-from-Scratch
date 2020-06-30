# AdaBoost-from-Scratch
Ada-boost or Adaptive Boosting is one of ensemble boosting classifier. It combines multiple classifiers to increase the accuracy of classifiers. AdaBoost is an iterative ensemble method. AdaBoost classifier builds a strong classifier by combining multiple poorly performing classifiers so that you will get high accuracy strong classifier. 

## Working of the Algorithm:
It works in the following steps:

**1.** Initially, Adaboost selects a training subset randomly.

**2.** It iteratively trains the AdaBoost machine learning model by selecting the training set based on the accurate prediction of the last training.

**3.** It assigns the higher weight to wrong classified observations so that in the next iteration these observations will get the high probability for classification.

**4.** Also, It assigns the weight to the trained classifier in each iteration according to the accuracy of the classifier. The more accurate classifier will get high weight.

**5.** This process iterate until the complete training data fits without any error or until reached to the specified maximum number of estimators.

**6**. To classify, we perform a "vote" across all of the learning algorithms we have built.

<img src="https://res.cloudinary.com/dyd911kmh/image/upload/f_auto,q_auto:best/v1542651255/image_3_nwa5zf.png">
<hr> </hr>

### Documentation of AdaBoost Classifier:
<a href="https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.AdaBoostClassifier.html">https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.AdaBoostClassifier.html </a>

<hr> </hr>

## Parameters of the Algorithm:
<ul>
  <li><b>base_estimator (default value = None)</b></li>
   It is a weak learner used to train the model. It uses DecisionTreeClassifier as default weak learner for training purpose. You can also specify different machine learning algorithms.
  <li><b> n_estimators (default=50)</b></li>
  Number of weak learners to train iteratively.
  <li> <b> learning_rate (default = 1) </b> <li>
 It contributes to the weights of weak learners.
  </ul>
 <hr>  </hr>
 
 ## Evaluation of the Model:
 ### a) Without Parameter Tuning:
                precision    recall  f1-score   support
          0       1.00      1.00      1.00        12
          1       0.79      0.94      0.86        16
          2       0.93      0.76      0.84        17
    avg / total   0.90      0.89      0.89        45
 
#### Accuracy: 0.8888888888888888
### b) After Parameter Tuning:
               precision    recall  f1-score   support
          0       1.00      1.00      1.00        12
          1       0.94      0.94      0.94        16
          2       0.94      0.94      0.94        17
    avg / total   0.96      0.96      0.96        45

#### Accuracy: 0.9555555555555556
