
## Introduction

Recognition of human activity is one of the active research areas in machine learning for various contexts such as safety surveillance, healthcare and human-machine interaction

Recognition of human activity is an ability to interpret the gestures or movements of the human body via sensors and to determine human activity or action. Most everyday human tasks can be simplified or automated if they can be recognized through the activity recognizing systems. Generally, the human activity recognition system may or may not be supervised.

The recognition of human activity is mainly used in health systems installed in the residential environment, hospitals and rehabilitation centres. It is widely used to monitor the activities of the elderly staying in rehabilitation centres for chronic disease management and disease prevention.


## Data Preprocessing

Now let’s start the task of Human Activity Recognition with machine learning by importing the necessary Python libraries

mport NumPy and pandas to manage tables and datasets. Then matplotlib is included to be used to create visualizations. To use various machine learning algorithms, I import SVM, Logistic Regression, K Nearest Neighbors Classifier, and Random Forest Classifier provided by Scikit-Learn. Also, accuracy_score is included to calculate the accuracy of the Activity Recognition Model.

There are a total of 7352 records in the training dataset. Also, there are no null values in the dataset. The test dataset contains 2947 records to test our models. This dataset does not have null values.

I can see that the dataset consists of accelerometer and gyro sensor values for each record. In addition, the last two columns are the subject which refers to the subject number and the activity which defines the type of activity. The Activity column will be represented by the label y and all other columns will be represented by X:


## Data Visualization

Now let’s visualize the data to understand some hidden features of the dataset:

The percentage of values shows that the size of the data for each activity is comparable. The dataset is also distributed. By inspecting the dataset, I can see that there are a lot of features.

It is easy to identify that there is an accelerometer, gyroscope, and other values in the data set. I can check everyone’s share by plotting a bar graph of each type. Accelerometer values have Acc in them, Gyroscope values have Gyro, and rest can be considered like others:

The accelerometer provides the maximum functionality, followed by the gyroscope. The other features are much less so.

If I take a closer look at the graph, we can see that each row on average transit between a maximum range of 0.2 to 0.3 values. This is indeed the expected behaviour as slight variations can be attributed to minor human errors.


## Summary

So we can clearly see that the Logistic Regression model performs the best for the task of Human Activity Recognition with Machine Learning.