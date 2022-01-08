# AmExpert_Hackathon_2021
### Problem Statement
A mid-sized private bank that includes a variety of banking products, such as savings accounts, current accounts, investment products, credit products, and home loans. The task is to predict the next set of products (upto 3 products) for a set of customers (test data) based on their demographics and current product holdings.

### Project Flow
* Importing the data
* EDA
* Feature Engineering / Data Preparation
* Splitting the data to train and test
* Feature Scaling
* Model Building
* Model Evaluation
* Prediction on Given Test Set

### Approach
* This is a Multi label Classification problem, where in we have to predict the top 3 products the customer will buy out of the 22 types of different products.
* Products (both B1 and B2) are converted to multi-hot encodings using MultiLabelBinarizer.
* One hot encoding is used to convert categorical variables to numeric (Gender, Customer_Category and City_Category)
* Age and Vintage Variables were scaled down by Normalization.
* Different ML models like Logistic Regression, XGBoost, CatBoost & ANN are used with Multioutputclassifier.
* Evaluation metrics used is average precision score.
* Finalised ANN model based on the evaluation metrics.

### Modeling
* Neural Network is used with with 3 hidden layers of 32,16,8.
* Relu Activation function is used for the input and the hidden layers.
* Sigmoid Activation function is used for the output layer.
* Adam optimizer is used for faster learning.
* Used BinaryCrossEntropy loss since it is a Multi Label problem.
* Avg_Precision_Score is used as evaluation matrix.
