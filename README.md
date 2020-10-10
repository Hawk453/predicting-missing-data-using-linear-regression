# Predicting missing data using linear regression
### The dataset contains missing values , we are trying to predict those values. After the processing we are able to generate a data set with the predicted values.</br>
For data scientists, handling missing data is an important part of the data cleaning and model development process. Often times, real data contains multiple sparse fields or fields that are laden with bad values. In this program, we have built models that can be used to impute missing or bad values in data.</br></br>
When the data set is analysed we face with a problem of missing data in ageEstimate  and redundant data in various labels which may impact our processing of the data.
Pre-processing is done to sort out the data by removing the redundant data and performing encoding on the categorical data to establish a metrics from where we can decide on a filter which we can use it to predict the missing data.</br></br>
After the data is processed we correlate the data against each other to find similarity.</br></br>
First let’s consider building a model that imputes missing ‘ageEstimate’ values using the ‘status’. To start, let’s correlate between ‘ageEstimate’ and ‘status’. We see that there is a weak correlation. Let’s build a linear regression model that uses ‘status’ to predict the ‘ageEstimate’. First, let’s import the ‘Linear Regression’ module from ‘scikit-learn’. Now let’s evaluate the performance of our model. Let’s use mean squared error to evaluate the performance of our model.</br> </br>
For comparison purposes we use various other models like Random Forests Regression, but in this scenario we had best possible predictions with Linear Regression.</br></br>

 _The process goes thus:</br>
Call the variable where you have missing values as y.</br>
Split data into sets with missing values and without missing values, name the missing set X_text and the one without missing values X_train and take y (variable or feature where there is missing values) off the second set, naming it y_train.</br>
Use one of classification methods to predict y_pred.</br>
Add it to X_test as your y_test column. Then combine sets together._
</br></br>
Further improvements can be done on this like hyperparameter tuning, and using a deep learning based network model which is explicitly designed for this.
