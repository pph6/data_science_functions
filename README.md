# Functions
A few statistical and data science functions, written in Python (Jupyter Notebook).
<br>
This document will outline the guidelines and parameters of the functions I have written in this repository. 


## 1. Empirical Random Variable: `empRV()`
A random variable (RV) is a function that maps all the elements of a sample space to real numbers. The empirical RV that this function outputs is the RV of the empirical probabilities of the input array. 

- Function parameters
  - Take in one input argument that represents a dataset in the form of a 1D numpy array. This array should contain a set of numbers of arbitrary size.
  - The function should return two outputs: First a 2D array with the first column being the sorted unique values in the dataset and in the 2nd column the associated probabilities. The second output should be the first moment (the expected value of this RV).


## 2. Mean Absolute Deviation: `MeanAbsDev()`
Sum of the deviations from the mean over size of sample (n).
--> need to put in formula image

- Function Parameters:
  - Take in one input argument that represents a dataset in the form of a 1D numpy array. This array should contain a set of numbers of arbitrary size.
  - The function should returns the median absolute deviation as an output.
