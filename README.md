# Romance-or-Thriller-Movie-Genre-Prediction-from-Audio-Visual-and-Text-Features
Testing different classification algorithms, experimenting with different features, and conducting a thorough evaluation

This file describes the Programming as part of 
COMP90049: Introduction to Machine Learning
Project 2: Movie Genre Prediction Based on Diverse Features and their Relationship with the Performance 

There are Two various Programing Files
1. Models.ipynb: consisting of predataprocession steps for all the datasets and implementation of the models
2. Visualization.ipynb: it is of the Model consisting of learning curve graph of each model.

# Models.ipynb

Running each cell in Jupter note book of these fuction.

Funcations:
1.load_data(): load the training and validation dataset datafiles and combine the datasets.

2.split_data_AV(x): It selects only the Audio and Video Features of the dataset [avg1 ... avg107 and ivec1 ... ivec20], preprocessing of the data. The function consist of
a prameter X which should be enterid while calling the function. valid inut of X : 'train_X', 'train_Y','test_X' and 'test_Y'.

3.split_data_word(X): It selects only the title, tag, Audio and Video Features of the dataset [movieTitle and Tag], preprocessing of the data. The function consist of
a prameter X which should be enterid while calling the function. valid inut of X : 'train_X', 'train_Y','test_X' and 'test_Y'.

4.split_data(X):It selects only the title and tag Features of the dataset [movieTitle, Tag, avg1 ... avg107 and ivec1 ... ivec20], preprocessing of the data. The function consist of
a prameter X which should be enterid while calling the function. valid inut of X : 'train_X', 'train_Y','test_X' and 'test_Y'.

5. Then other fuctions are implementation of the models and evaluation of each model.

# Visualization.ipynb

Running each cell in Jupter note book of these fuction.

Funcations: These are similar funcation to that of Models.ipnb but the implementation of the funcation are different.

1.load_data(): load the training and validation dataset datafiles and combine the datasets.

2.split_data_AV(x): It selects only the Audio and Video Features of the dataset [avg1 ... avg107 and ivec1 ... ivec20], preprocessing of the data. The function consist of
a prameter X which should be enterid while calling the function. valid inut of X : 'X and 'Y'.

3.split_data_word(X): It selects only the title, tag, Audio and Video Features of the dataset [movieTitle and Tag], preprocessing of the data. The function consist of
a prameter X which should be enterid while calling the function. valid inut of X : 'X', 'Y'.

4.split_data(X):It selects only the title and tag Features of the dataset [movieTitle, Tag, avg1 ... avg107 and ivec1 ... ivec20], preprocessing of the data. The function consist of
a prameter X which should be enterid while calling the function. valid inut of X : 'X' and 'Y'.

5.plot_learning_curve() Generate a simple plot of the test and traning learning curve. 
    
    Parameters
    ----------
    estimator : object type that implements the "fit" and "predict" methods
        An object of that type which is cloned for each validation.

    title : string
        Title for the chart.

    X : array-like, shape (n_samples, n_features)
        Training vector, where n_samples is the number of samples and
        n_features is the number of features.

    y : array-like, shape (n_samples) or (n_samples, n_features), optional
        Target relative to X for classification or regression;
        None for unsupervised learning.

    ylim : tuple, shape (ymin, ymax), optional
        Defines minimum and maximum yvalues plotted.

    cv : integer, cross-validation generator, optional
        If an integer is passed, it is the number of folds (defaults to 3).
        Specific cross-validation objects can be passed, see
        sklearn.cross_validation module for the list of possible objects

    n_jobs : integer, optional
        Number of jobs to run in parallel (default 1).
  --------

5. Reset of the code is on different cells calling the function plot_learning_curve(with different paraments)
