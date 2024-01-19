# Classification Method Visualization Project
The following classification methods were trained and their accuracies were visualized on a line plot: 
* Linear
* K-Nearest Neighbors
* Random Forest
* Naive Bayesian

Jupyter Notebook was used to write and test the Python code.

The following Python libraries were used:
* mathplotlib - for visualization
* scikit-learn - for creating the models
* numpy - array manipulation

For each of the 4 data sets, a new instance classifications method was created. Each classification method was 
then trained on the training data. The accuracy of the train and test data was then visualized using a line plot. 

## Test Accuracies of All 4 Classifiers Across All 4 Datasets
<img width="420" alt="Screen Shot 2024-01-19 at 3 52 10 PM" src="https://github.com/eeshaarabhavi/DS-Project/assets/56767468/06e66f55-b6fd-42d6-bfab-90b657b1a2c2">

Using this graph above, I came to the following conclusions about my results:

### Dataset 1
This dataset has some x values that are negative in both the training and testing data. Although the Random Forest 
Classifier seems to be the best in terms of training accuracy for each dataset, this is not always the case since Random 
Forests tend to overfit so tuning the hyperparameter of nestimators would give a more accurate model for each dataset. The x 
data in this dataset has dimension of 2 which is countered by there being a large number of datapoints which makes KNN a valid 
model but overfitting is always still possible with KNN. In contrast, Gaussian Naive Bayes Classifiers are very good at handling 
large amounts of data while also not overfitting. Linear Classifier only is effective with data in datasets that are linear in 
nature but after viewing this dataset, I observed that the data are not exactly linear in nature. Due to this, the linear classifier
did not accurately model both the training and test data.

### Dataset 2
This dataset has no negative x values in both the training and the testing data unlike Dataset 1. The Random Forest Classifier 
training accuracy for all of the datasets seems to be similar and this could be because the hyperparameter nestimators needs to be 
tuned for each dataset so that the Random Forest Classifier does not overfit the data. Due to a large amount of datapoints in the 
dataset compensating for the dimensionality of the data, this data can be modeled using KNN classifier but there is still also a 
possibility of overfitting. Additionally, the testing accuracy for the Linear Classifier being high tells us that the dataset is more 
linear than the other datasets. The Gaussian Naive Bayes Classifier has the same test and training accuracies as the Linear Classifier 
and this could be because they are both the best model for this dataset.

### Dataset 3
This dataset has a large dimensionality but the number datapoints in the dataset are not exponentially larger which means that KNN 
classifier cannot be a good model for the data. Further more, as stated above, the Random Forest Classifier's hyperparameter 
nestimators needs to tuned for this dataset inorder for the classifier to not overfit the data. This is because the Random Forest 
Classifier's training accuracy for all of the datasets is very high which means that the classifier's hyperparameter has not been 
tuned for each dataset. The Linear Classifier's testing accuracy being low could be because the data was not linear in nature. Thus 
using a Gaussian Naive Bayes Classifier would give a more valid model for this dataset.

### Dataset 4
This dataset has a large dimensionality but again like dataset 3, the number of datapoints in the dataset are not exponentially larger 
which means that the KNN classifier cannot be a good modeel for the data. Furthermore, as mentioned before, the Random Forest Classifier 
training accuracy for all of the datasets seems to be similar and this could be because the hyperparameter nestimators is not tuned for 
the dataset to make sure that the Random Forest Classifier does not overfit the data. The Gaussian Naive Bayes Classifier and the Linear 
Classifier have the same testing accuracy but not the same training accuracy. Since testing accuracy is more important than training 
accuracy when figuring out which model is the best model for the dataset, both the Linear Classifier and the Gaussian Naive Bayes 
Classifier would probably be valid models.


