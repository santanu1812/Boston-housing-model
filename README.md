# Linear-regression-from-scratch
### I have implemented a Linear regression model built from scratch, without using any machine learning python libraries like scikit-learn,keras, tensorflow or PyTorch
This is my first machine learning project.
The model is trained and implemented on the [boston housing dataset](https://www.kaggle.com/datasets/krupadharamshi/bostonhousing) by selectively using the following features to predict the **"medv"-median value of house**-
- **"crim"**-per capita crime rate by town
- **"rm"**-Average number of rooms per dwelling
- **"age"**-Proportion of owner-occupied units built prior to 1940
- **"dis"**-Weighted distances to five Boston employment centers
- **"rad"**-Index of accessibility to radial highways
The advantage of my model is that, it can be expanded to any number of features with little to no changes to the code
---
### PROJECT HIGHLIGHTS
- No use of machine learning libraries
- Manual feature normalization(z-score)
- Custom **Root mean-squared error(RMSE)** and **Coefficient of determination(R^2)**
- prediction plot to visualize the model's performance
- the code is written in the simplest possible manner, such that even a beginner in ML can have a good grasp of the operations
---
### LIBRARIES USED
- Numpy- *for basic math and array operations* 
- seaborn and matplotlib-  *for visualizing the dataset and models output*
- pandas-*for reading the csv file and preseting the data in a readable way*
- random-*to generate random values for initializing the parameters*
---
### R^2 score on the test set: 0.7200 
**The R^2 score may vary slightly in each run due to the use of random.shuffle() to split the train-test datasets**
>The RMSE of the model doesnt converge near 0 values, because of the noise in the dataset.
>The performance of the model is decent, considering it only uses basic linear regression model with no sophisticated libraries

