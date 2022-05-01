# Ensemble Learning

## Ensemble Methods
Ensemble methods are machine learning methods that aggregate the predictions of a group of base learners in order to form a single learning model. For example, imagine that each person in this video is a trained machine learning model and notice the average of their predictions is a much more accurate prediction that the individual predictions. In this lecture we will consider two types of ensemble concepts and methods. Namely,

- Bagging

- Random Forests

### Bagging

The term bagging referes to bootstrap aggregating. Bootstrapping is a method of inferring results for a population from results found on a collection of smaller random samples of that population, using replacement during the sampling process. In the context of machine learning, a given set of machine learning model is trained respectively on random samples of training data with replacement (see the above figure), then the combined predictions of each model is aggregated and used as a single prediction. For regression tasks this would mean taking the average of the set of model prediction, and for classification taking the majority vote.

Generally speaking, the models we pick for ensembling will be "dumb learners", meaning models that are barely superior to randomly guessing. Individually the models will perform poorly, but collectively will perform well.

### Random forests

Technically speaking, the above bagging model is called a Random forest. Such a model exists inside the sklearn.ensemble module, and is the DecisionTreeClassifier class. However, the random forest algorithm used in training the RandomForestClassifier class introduces extra randomness when growing trees; instead of searching for the best feature when splitting a node, it searches for the best feature among a random subset of features. This results in a greater diversity of trees which results in even lower variance of the fit model.

## Ensemble Boosting

Boosting is an ensemble method that trains predictors sequentially, each trying to correct the errors made by the previous predictor. In this lecture we consider two well known boosting methods, namely AdaBoost and gradient boosting.

### AdaBoost

With AdaBoost, the training algorithm first trains a base classifier and uses it to make predictions on the training set. Then, each of the missclassified training instances is then given a relative weight. The next classifier is then trained on the dataset using these relative weights, and so on.

The idea is that whenever a classifier missclassifies a data point,this data point is then boosted to signal difficulty in classification.

### Gradient Boosting

Another popular boosting method is gradient boosting. This method works by sequentially adding predictors to an ensemble, each correcting is predecessor. The difference between this method and AdaBoost is that gradient boosting tries to fit the new predictor to the residual errors made by the previous predictor.

## Datasets

### Palmer Penguins
source: @allison_horst https://github.com/allisonhorst/penguins

The Iris flower data set or Fisher's Iris data set is a multivariate data set introduced by the British statistician and biologist Ronald Fisher in his 1936 paper The use of multiple measurements in taxonomic problems as an example of linear discriminant analysis[source:WIkipedia]

Palmer Archipelago (Antarctica) penguin dataset appears to be a drop in replacemnt for the same. It is a great intro dataset for data exploration & visualization. Let's import the dataset and explore it to understand it better.
