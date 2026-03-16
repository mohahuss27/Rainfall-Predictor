# Rainfall Predictor

## Overview
This project implements a machine learning model to predict whether it will rain tomorrow based on historical weather data for Melbourne and nearby areas (MelbourneAirport, Watsonia). The model uses a Random Forest Classifier optimized via Grid Search Cross-Validation.

## Dataset
- Source: [weatherAUS-2.csv](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/_0eYOqji3unP1tDNKWZMjg/weatherAUS-2.csv)
- Description: Australian weather dataset with features like temperature, humidity, wind speed, etc.
- Preprocessing: Drops null values, filters locations, extracts seasons from dates, and balances the target variable.

## Project Highlights
- Predicted next-day rainfall with **86% accuracy**.
- End-to-end workflow: data preprocessing → feature engineering → model training → evaluation.
- Evaluation metrics: precision, recall, F1-score, and confusion matrix.
  
## Dependencies
- pandas
- scikit-learn

Install via pip:
```
pip install pandas scikit-learn
```

## Usage
1. Open `Rainfall_predictor.ipynb` in Jupyter Notebook or VS Code.
2. Run the cells sequentially to load data, preprocess, train the model, and evaluate.
3. The notebook outputs the best model parameters, validation score, classification report, and confusion matrix.

## Model Details
- Algorithm: Random Forest Classifier
- Hyperparameter Tuning: Grid Search with Stratified K-Fold CV
- Features: Numerical (scaled) and categorical (one-hot encoded)
- Target: RainTomorrow (binary classification)

## Results
- Best parameters and score are printed after training.
- Evaluation metrics include precision, recall, F1-score, and accuracy on the test set.
- Confusion matrix visualization is generated.

## Contributing
Feel free to fork and submit pull requests for improvements.

## License
This project is for educational purposes. Check the dataset license for usage restrictions.
