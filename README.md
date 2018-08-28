# Titanic_Kaggle
the goal is to predict the survival or the death of a given passenger based on 12 feature such as sex, age ,etc...
what will you read in this tutorial?
# 1 Define Problem
2 Installation
3 Import Machine learning libraries
4 EDA
5 Feature Engineering
6 Modeing
7 Feature Selection
8 Conclusion
# 1- Define Problem
# 1-1 introduction
RMS Titanic was a British passenger liner that sank in the North Atlantic Ocean in the early hours of 15 April 1912, after colliding with an iceberg during its maiden voyage from Southampton to New York City. There were an estimated 2,224 passengers and crew aboard, and more than 1,500 died, making it one of the deadliest commercial peacetime maritime disasters in modern history. RMS Titanic was the largest ship afloat at the time it entered service and was the second of three Olympic-class ocean liners operated by the White Star Line. It was built by the Harland and Wolff shipyard in Belfast. Thomas Andrews, her architect, died in the disaster.

# 1-2 dataset
Titanic dataset is an open dataset where you can reach from many different repositories and GitHub accounts. However, downloading from Kaggle will be definitely the best choice as the other sources may have slightly different versions and may not offer separate train and test files. So, please visit this link to download the datasets (Train.csv and Test.csv) to get started.

# 2- installation
A very easy way to install these packages is to download and install the Conda distribution that encapsulates them all. This distribution is available on all platforms (Windows, Linux and Mac OSX).

# 3- Import
Throughout this jupyter notebook, I will be using Python at each level of the pipeline.

The main libraries involved in this tutorial are:

Pandas for data manipulation and ingestion
Matplotlib and seaborn for data visualization
Numpy for multidimensional array computing
sklearn for machine learning and predictive modeling
# 4 - Exploratory data analysis
As in different data projects, we'll first start diving into the data and build up our first intuitions.

In this section, we'll be doing four things.

Data extraction : we'll load the dataset and have a first look at it.
Cleaning : we'll fill in missing values.
Plotting : we'll create some interesting charts that'll (hopefully) spot correlations and hidden insights out of the data.
Assumptions : we'll formulate hypotheses from the charts.
I am assuming that you have your Python3 environment installed.

# 4-1 Load data
# 4-2 shape of data
# 4-3 Head of data
# 4-4 Features
The Survived column is the target variable. If Suvival = 1 the passenger survived, otherwise he's dead. The is the variable we're going to predict.

The other variables describe the passengers. They are the features.

PassengerId: and id given to each traveler on the boat
Pclass: the passenger class. It has three possible values: 1,2,3 (first, second and third class)
The Name of the passeger
The Sex
The Age
SibSp: number of siblings and spouses traveling with the passenger
Parch: number of parents and children traveling with the passenger
The ticket number
The ticket Fare
The cabin number
The embarkation. This describe three possible areas of the Titanic from which the people embark. Three possible values S,C,Q
# 4-5 Data describe
Pandas allows you to a have a high-level simple statistical description of the numerical features. This can be done using the describe method.
The count variable shows that 177 values are missing in the Age column. One solution is to fill in the null values with the median age. We could also impute with the mean age but the median is more robust to outliers.
# 4-6 Charts
let's now make some charts.
let's visualize survival based on the gender
