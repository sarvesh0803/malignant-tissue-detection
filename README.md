# Malignant tissue detection for Breast Cancer
Classify images of tissues possibly affected with breast cancer using characteristics extracted from tissue cells.

## Objective
The objective is to classify the Wisconsin Diagnostic Breast Cancer(WDBC) dataset to separate __malignant tissues__ from __benign tissues__. We would want to estimate the misclassification rates of both classes and populate the 2x2 confusion matrix. Furthermore, we would wish to maximize the __true-positives__ and minimize the __false-negatives__.

## Understanding the dataset
The Wisconsin Diagnostic Breast Cancer(WDBC) dataset is available in the the UCI repository. Each row in the dataset represents a sample of biopsied tissue. The tissue for each sample is imaged and 10 characteristics of the nuclei of cells present in each image are characterized.


There are four `csv` files in the dataset. Two files are used for training our model and the other two for test. The files have been appropriately and distinctively named `trainX`, `trainY`, `testX`, `testY`. The `X` label stands for dataset of the samples with the features and the `Y` stands for the associated label for each sample.


A label of value 1 indicates the sample was for malignant (cancerous) tissue, 0 indicates the sample was for benign tissue.

## Features

  - The characteristics in the dataset are: Radius, Texture, Perimeter, Area, Smoothness, Compactness, Concavity, Number of concave portions of contour, Symmetry, Fractal dimension.
  - Each sample used in the datasetis a feature vector of length 30. 
  - The first 10 entries in this feature vector are the mean of the characteristics listed above for each image. 
  - The second 10 are the standard deviation and last 10 are the largest value of each of these characteristics present in each image
  
## Jupyter notebook

  - You can either check out the notebook [here](http://nbviewer.jupyter.org/github/sarvesh0803/malignant-tissue-detection/blob/master/Malignant%20tissue%20detection%20for%20Breast%20Cancer.ipynb)
  - Or you can download and run it locally
  - You will need `python3`, `pip`, `jupyter` and these libraries:
    - numpy
    - scipy
    - sklearn
    - sklearn.metrics
    - seaborn
    - pandas
    - graphviz
    - matplotlib.pyplot
  - I recommend using [Anaconda](https://www.anaconda.com/download/) for easy installation
  - The code is well commented and explained in the notebook
