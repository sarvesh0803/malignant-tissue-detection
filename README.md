# Malignant tissue detection for Breast Cancer
Classify images of tissues possibly affected with breast cancer using characteristics extracted from tissue cells.

## Objective
The objective is to classify the Wisconsin Diagnostic Breast Cancer(WDBC) dataset to separate __malignant tissues__ from __benign tissues__. We would want to estimate the misclassification rates of both classes and populate the 2x2 confusion matrix. Furthermore, we would wish to maximize the __true-positives__ and minimize the __false-negatives__.

## Understanding the dataset
Wisconsin Diagnostic Breast Cancer(WDBC) dataset from the UCI repository. Each row in the dataset represents a sample of biopsied tissue. The tissue for each sample is imaged and 10 characteristics of the nuclei of cells present in each image are characterized.


There are four `csv` files in the dataset. Two files are used for training our model and the other two for test. The files have been appropriately and distinctively named `trainX`, `trainY`, `testX`, `testY`. The `X` label stands for dataset of the samples with the features and the `Y` stands for the associated label for each sample.

## Features

  - The characteristics in the dataset are: Radius, Texture, Perimeter, Area, Smoothness, Compactness, Concavity, Number of concave portions of contour, Symmetry, Fractal dimension.
  - Each sample used in the datasetis a feature vector of length 30. 
  - The first 10 entries in this feature vector are the mean of the characteristics listed above for each image. 
  - The second 10 are the standard deviation and last 10 are the largest value of each of these characteristics present in each image
  
