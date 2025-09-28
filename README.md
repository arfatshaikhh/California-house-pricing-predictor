# California-housing-prices-predictor
This project is an end-to-end machine learning pipeline for predicting housing prices in California.

It takes raw housing data, preprocesses it (cleaning, scaling, encoding), trains a Random Forest regression model, and allows easy inference on new data. Both the preprocessing pipeline and trained model are saved, so the workflow is fully reusable.


*What the  project Does

Preprocessing

Handles missing values (median imputation)

Scales numerical features

One-hot encodes categorical features

Data Splitting

Uses StratifiedShuffleSplit to create balanced train/test sets by income category

Model Training

Trains a RandomForestRegressor

Saves the trained model (model.pkl) and preprocessing pipeline (pipeline.pkl)

Inference

Loads saved pipeline + model

Transforms new input data (input.csv)

Outputs predictions (output.csv)


*How to Run the project

1️⃣ Train the model

code:python main.py


it will Splits dataset,Preprocesses features,Trains model and saves artifacts.

2️⃣ Run inference

code:python main.py


If model.pkl exists → skips training,Loads input.csv,Saves predictions in output.csv.


*Built With: Python 3.x, pandas, numpy, scikit-learn, joblib


*Use Cases

1)Estimating housing prices for real estate companies

2)Assisting buyers and sellers in understanding market trends

3)Providing a base pipeline for students and researchers to experiment with ML workflows


