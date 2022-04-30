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

## 3. Normalized Error: `normalized_error()`
RMSE (Root Mean Squared Error) is a common measure guaging the accuracy of machine learning models, but it is not all-encompassing. If dealing wiht ordinal or data witha lot of outliers then we might be better off using mean absolute deviation instead. So I am writing here a general normalized error function.

- Function Parameters:
  - Take in two arguments/inputs, in this order: 1) An input dataset (make it a 2D numpy array or dataframe), 2) a flag by which power to normalize the error, for instance 1 for the mean absolute error, 2 for the RMSE, 3 for the cubic root mean cubed error and so on.
  - Calculate the error of the input array in a1, normalized by the flag set in a2, according to the following general equation: 
  𝑁𝐸 =   [ ∑( | 𝑌̂𝑖  − 𝑌𝑖 | )^𝑝 / 𝑛]^(1/𝑝) ----------> insert picture
 where  𝑌̂ are the predictions, 𝑌 are the measurements, p is the power specified in a2, n is the number of rows of the array in a1, and i is the ith row, from 1 to n, yielding the normalized error NE. 
  - The function will return the output of this calculation should be a single scalar, real number.
  - Assumptions: 
    -  You can assume that the input will be a 2D array (with predictions in the column 1 and
measurements in column 
    - The number of rows of this input array should be flexible/up to the user.

## 4. 
