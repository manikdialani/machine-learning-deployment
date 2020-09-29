# Machine Learning Deployment Tutorials
Launch machine learning models into production using flask, docker etc.

## Environment and tools
1. scikit-learn
2. pandas
3. numpy
4. flask

## Installation

`pip install scikit-learn pandas numpy flask`

`python model.py`

`python app.py`

![Logo](i1.png)

# 2. Predict Prices

Download the dataset from [here](https://www.kaggle.com/shivachandel/kc-house-data).

## Environment and tools
1. scikit-learn
2. pandas
3. numpy
4. flask
5. docker

## Installation

`docker-compose up --build`

`curl -X POST -H "Content-Type: application/json" -d @to_predict_json.json http://localhost:8080/predict_price`

where `to_predict.json` contains:

`{"grade":9.0,"lat":37.45,"long":12.09,"sqft_living":1470.08,"waterfront":0.0,"yr_built":2008.0}`

or

`curl -X POST -H "Content-Type: application/json" -d '{"grade":9.0,"lat":37.45,"long":12.09,"sqft_living":1470.08,"waterfront":0.0,"yr_built":2008.0}' http://localhost:8080/predict_price`
#
Credits to: Abhinav Sagar

