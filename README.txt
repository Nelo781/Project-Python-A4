------------------------------------------------------------------------------------------------------------------

Identify copyist of “Avila Bible” with Supervised Learning

This project takes place for the Python Course Final Project of the ESILV DIA degree 2020/2021.


This is a classification project in python based on the Avila Bible Dataset. The
purpose is to predict the copysist for each of the 10429 Avila Bible samples,
depending on the several features contained in the dataset for each sample.

The data is divided in 2 set: avila_tr the training set used for fitting the classifiers
and the avila_ts, the test set used for validation.

You can find the Python Notebook in wich we used scikit learn classifiers for
classication and seaborn for visualization.

We trained several classification methods as:
  - Linear Discriminant Analysis
  - Decision Tree
  - Random Forest
  - Grid Search: Random Forest
  
We also used the scikit learn confusion matrix, accuracy score and cross-validation
to dertermine the most accurate method(s) for this classification project.

We attached to this repositorie the report of our work explaining our quest 
of accuracy.

----------------------
Flask API

To develop our API we decided to do it with Flask because we already had the knowledge to do it.

First of all, we generated a pickle file that represents our most powerful model, it's thanks to that we will be able to create a prediction API.
To start with, we made a virtual environment for the API to install the prerequisites that were in a requirement.txt : flask, pandas and scikit learn.
We then developed simultaneously the python code that represents the API and the html file that will be a web page where we will be able to indicate the different variables and then have the result of the prediction.

For the python code we used flask to do this, we use the 'POST' method to retrieve the variables specified on the web page which was generated thanks to the html file we imported into the code. 
After the values put on the page and submit, we import the model with the pickle file and we store all the values in variables, we had to initialize all of them with an if else to have no value None, then we then put in an array that will be the variable to predict the result.
The prediction is then calculated thanks to the model and then retrieved to display it on the page thanks to the html file.

The html file is a form in 'POST' method to retrieve all the variables we are going to fill in. 
Then we have in text zones each variable that we will have to fill in to predict the copyist and a submit button to send all of them to the API. 
At the end, we have added the result of the prediction we made beforehand by recovering it from the python code. 

----------------------

We hope you'll enjoy it !

Jules & Stéphane
