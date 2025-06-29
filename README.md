# Linear-regression-from-scratch
#### I have implemented a Linear regression model built from scratch, without using any machine learning python libraries like scikit-learn,keras, tensorflow or PyTorch
This is my first machine learning project.\
The model is trained and implemented on the [boston housing dataset](https://www.kaggle.com/datasets/krupadharamshi/bostonhousing) by selectively using the following features to predict the **"medv"-median value of house**-
- **"crim"**-per capita crime rate by town
- **"rm"**-Average number of rooms per dwelling
- **"age"**-Proportion of owner-occupied units built prior to 1940
- **"dis"**-Weighted distances to five Boston employment centers
- **"rad"**-Index of accessibility to radial highways
The advantage of my model is that, it can be expanded to any number of features with little to no changes to the code
---
### WHY THIS PROJECT MATTERS
most machine learning projects today rely on black-box models.This project intentionally takes the *opposite route* in order to offer an easy interpretable and fine grained understanding of:
- how linear models learn the patterns from the data
- how we can optimize our model to make it less-sensitive to outliers
- how the different models perform in a noisy dataset
> this project was built when i was a complete beginner in this field, which ensures it can be understood by a complete beginner with little effort
---
### CORE TECHNIQUES IMPLEMENTED
#### LINEAR REGRESSION
- Feature normalization(z-score method)
- Gradient descent with manual convergence control
- proper visualization of the *loss vs epochs* and the outcomes of the model
- using the R^2 metric to compute the efficiency of the model
#### LIBRARIES USED
- **Numpy**- for basic math and array operations
- **seaborn and matplotlib**-  for visualizing the dataset and models output
- **pandas**-for reading the csv file and preseting the data in a readable way
- **random**-to generate random values for initializing the parameters
- **os**-to create and store certain values in a directory, to be used across different models
--- 
**The R^2 score may vary slightly in each run due to the use of random.shuffle() to split the train-test datasets**
>The RMSE of the model doesnt converge near 0 values, because of the noise in the dataset.
>The performance of the model is decent, considering it only uses basic linear regression model with no sophisticated libraries
---
### UPDATE 1:
> introducing robust regression using Hubers loss, which optimizes the model by making it less-sensitive to outliers
- Uses a search algorithm to find the optimum value of *delta* for which the R^2 metric is maximum ( or the efficiency is maximum)
- comparative analysis with the standard linear regression model
---
### UPDATE 2:
>added a linear regression model using scikit learn for comparing the result with my own model
- Uses *LinearRegression* class from the *sklearn.linear_model* module.
- The r2 score of this model is almost same as my previous model, and lesser than the Robust regression model


