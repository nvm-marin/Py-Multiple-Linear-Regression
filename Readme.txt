This code showcases the implementation of a Multiple Linear Regression model in Python, utilizing the scikit-learn library.
Moreover it aims to predict a target variable based on multiple independent variables. It involves data import, preprocessing, and encoding steps to prepare the data for training the regression model,
demonstrates the basic workflow of the model without dividing the data into training and testing sets.

Comments:
1. Data Import and Preprocessing:
  -The code begins by importing essential libraries, including numpy, matplotlib.pyplot, and pandas.
  -It proceeds to read the data from the 'Data.csv' file, storing it in a pandas DataFrame called dataset.
2.Data Encoding:
  -To handle categorical variables, the code employs scikit-learn's ColumnTransformer and OneHotEncoder.
  -Specifically, it performs one-hot encoding on the categorical variable at index 3 within the X array.  
3. Train-Test Split:
   -To evaluate the model's performance, the code employs train_test_split from scikit-learn, splitting the data into training and testing sets.
   -The training set comprises 80% of the data (X_train and y_train), while the remaining 20% is allocated to the testing set (X_test and y_test).
 4. Model Training and Prediction:
   -The code initializes a LinearRegression model from scikit-learn.
   -It proceeds to fit the model to the training data (X_train and y_train) using the fit method.
   -The trained model is then employed to predict the target variable for the test data (X_test), with the predictions stored in y_pred.

Developer: @marincolta
