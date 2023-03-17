# MLOps E2E Workflow -- Boston House Price Prediction Using Linear Regression 

## Problem Statement 

To predict the house prices based on other features like Number of rooms, Age of the property etc.

<br>

## Dataset

The Dataset used is the Housing dataset which contains information about different houses in Boston. This data was originally a part of UCI Machine Learning Repository and has been removed now. We can also access this data from the scikit-learn library and kaggle. There are 506 samples and 13 feature variables in this dataset. The objective is to predict the value of prices of the house using the given features.

<br>

## Check out The Application

Demo - https://lr-houseprice.onrender.com

*Note* - If the link doesn't give a quick response on click, copy and past it in a new tab and wait. It's a bit laggy on intial call but will work fine once the page loads up once. 

<br>


## Web Interface

<img width="1440" alt="Screenshot 2023-02-24 at 3 37 47 PM" src="https://user-images.githubusercontent.com/114252357/221287962-a5097e72-4ae3-4899-b5e7-cf71388c88cd.png">


<br>
<br>


##  Steps to Deploy the Application

## 1)  Local Deployment

#### 1) Clone the repostory 

```
git clone https://github.com/Pratik-Prakash-Sannakki/Plug-n-Predict_MLOps.git

```
#### 2) Create a conda Environment 

```
conda create -n {Environment name} python==3.7 

```

#### 3) Start the Environment 

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

<br>


## 2)  Cloud Deployment


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
<br>
<br>


## Steps to Build the Application 

#### 1)  Notebook

##### Highlights of the notebook 

1)  Library and Dataset Imports 
2)  Exploratory Data Analysis
3)  Train and Testing the model
4)  Saving the model

*Colab link to run the notebook on its own* - https://colab.research.google.com/drive/1hzrcfCEe3q7H8VywgXoOKg91e1_-QBNj?usp=sharing

*Note* - More elaborate cell by cell explaining given in the notebook

#### 2) Flask Web Application

An app.py file is created to define endpoints which intern triggers the Predictor function. The Predictor function containing the imported model and predicts the House price based on data input provided by the user from the Web interface. 

#### 3)  Application Front End  

An predict.html file which contains code for a form for the user to enter data.

#### 4)  Requirements File

A requirements.txt which contains all the library required to run the application.




