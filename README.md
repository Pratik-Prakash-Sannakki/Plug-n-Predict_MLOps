# MLOps E2E Workflow -- Boston House Price Prediction Using Linear Regression 

## Problem Statement 

To predict the price of the houses Price based on other features like Number of rooms, Age of the property etc.

## Dataset

The Dataset used is the Housing dataset which contains information about different houses in Boston. This data was originally a part of UCI Machine Learning Repository and has been removed now. We can also access this data from the scikit-learn library and kaggle. There are 506 samples and 13 feature variables in this dataset. The objective is to predict the value of prices of the house using the given features.

##  Steps to Deploy the Application

### 1)  Local Deployment

#### 1) Clone the repostory 

```
git clone https://github.com/Pratik-Prakash-Sannakki/MLOps_E2E_Workflow_LinearRegression.git

```
#### 2) Create a conda Environment 

```
conda create -n {Environment name} python==3.7 

```

### 3) Start the Environment 

```
conda activate {Environment name} 

```

#### 4) Install requirements

```
pip install requirements.txt

```

#### 5) Run the Application 
```
python app.py

```

#### 6)  Access the local Web Application  

   copy the url eg. 127.0.0.1/5000 from the out put and paste the URL in your browser 


### 1)  Cloud Deployment
---

#### 1) Clone the repostory 

```
git clone https://github.com/Pratik-Prakash-Sannakki/MLOps_E2E_Workflow_LinearRegression.git

```
#### 2) Create a git repository with all the cloned file  
#### 3) Create a Render Account 
  link - https://render.com/
#### 4) link you github account and create a new Web service
#### 5) connect your git Repository 
#### 6) Change name of API to your desired name and change start command to
```
gunicorn {flask file name}:app

```
#### 7) Deploy the application 

#### 8) Go to the URL provided on deployment 

#### 9) Now you can access the application remotely


## Step to Build the Application 

### 1)  Creation of a notebook for prediction 

#### Highlights of the notebook 

1)  Library and Dataset Imports 
2)  Exploratory Data Analysis
3)  Train and Testing the model
4)  Saving the model

**Colab link to run the notebook on its own** - https://colab.research.google.com/drive/1hzrcfCEe3q7H8VywgXoOKg91e1_-QBNj?usp=sharing

**Note** - More elaborate cell by cell explaining given in the notebook

### 2) Create a Flask application

An app.py file is created to define endpoints which intern triggers the Predictor function. The Predictor function containing the imported model and predicts the House price based on data input provided by the user from the Web interface. 

### 3)  Create a Home HTML file for the Web Interface  

An predict.html file which contains a form for user to enter data.

### 4)  Create a Requirements File

A requirements.txt which contains all the library reuired for the application to predict.

### 5)  
