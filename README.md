# Flight Fare Prediction: 

## Table of Content
  * [Demo](#demo)
  * [Overview](#overview)
  * [Installation](#installation)
  * [Deployement on Heroku](#deployement-on-heroku)
  * [Directory Tree](#directory-tree)
  * [Future scope of project](#future-scope)


## Demo
Link: [https://flight-price-prediction-api.herokuapp.com/](https://flight-price-prediction-api.herokuapp.com/)

![image](https://user-images.githubusercontent.com/91054745/134035457-0e795315-b913-41fe-82a0-cf2c35d399d8.png)
![ds2](https://user-images.githubusercontent.com/91054745/134035535-b14c5c4e-bea1-45e5-9c11-a351beab2c34.jpg)


## Overview
This is a Flask web app which predicts fare of Flight ticket.

## Methodology

* We started with data exploration and found out that there were 16 columns. Then we moved on to cheking if there were any null values. One row was removed thereafter.
* We then did Data Visualisation using seaborn and matplotlib libraries.
* Then we moved on to Data Prepocessing. WE saw that there were categorical values and hence we have to encode them. We used Label Encoder and One Hot Encoding.
* Thereafter we had 45 columnns when we created dummy variables.
* We used regex to process dates and time in order to convert data into the form over which a model could be trained.
* In this we kept the test abd train data separate to avoid Data Leak.
* Then we used Random Forest Classifier model over the dataset.
* We obtained 81% accuracy.
* Then we created the pickle file to Dump(save) the model.

## Installation
The Code is written in Python 3.6.10. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:
```bash
pip install -r requirements.txt
```

## Deployement on Heroku
Login or signup in order to create virtual app. You can either connect your github profile or download ctl to manually deploy this project.

[![](https://i.imgur.com/dKmlpqX.png)](https://heroku.com)

Our next step would be to follow the instruction given on [Heroku Documentation](https://devcenter.heroku.com/articles/getting-started-with-python) to deploy a web app.

## Directory Tree 
```
├── static 
│   ├── css
├── template
│   ├── home.html
├── Procfile
├── README.md
├── app.py
├── flight_price.ipynb
├── flight_rf.pkl
├── requirements.txt
```

## Technologies Used

![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://flask.palletsprojects.com/en/1.1.x/_images/flask-logo.png" width=170>](https://flask.palletsprojects.com/en/1.1.x/) [<img target="_blank" src="https://number1.co.za/wp-content/uploads/2017/10/gunicorn_logo-300x85.png" width=280>](https://gunicorn.org) [<img target="_blank" src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" width=200>](https://scikit-learn.org/stable/) 


## Future Scope

* Use multiple Algorithms
* Optimize Flask app.py
* Front-End 
