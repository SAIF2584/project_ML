# Bangalore House Price Prediction

## Project Overview

This repository contains a machine learning project for predicting real estate prices in Bangalore, India. The project uses a dataset of residential properties to build and evaluate regression models that estimate property prices based on features such as location, square footage, number of bedrooms, and bathrooms.

## Contents

- `project_01/Real_Estate_Price_Prediction.ipynb` - Jupyter notebook with data exploration, preprocessing, feature engineering, outlier handling, model training, and evaluation.
- `project_01/Bengaluru_House_Data.csv` - Raw housing dataset used for analysis.
- `project_01/bhp.csv` - Cleaned dataset generated during preprocessing.
- `project_01/columns.json` - JSON file containing model feature column names.
- `project_01/banglore_home_prices_model.pickle` - Trained machine learning model saved for later use.
- `requirements.txt` - Python dependencies for reproducing the analysis.

## Key Steps

1. Load the dataset and inspect missing values.
2. Drop unused columns and clean data.
3. Convert area values to numeric and compute price per square foot.
4. Group locations and reduce rare categories.
5. Remove outliers based on square footage and price per square foot.
6. Encode categorical location data using one-hot encoding.
7. Train and evaluate regression models, including cross-validation.
8. Use `GridSearchCV` to find the best model hyperparameters.

## Dependencies

Install the required dependencies using:

```bash
pip install -r requirements.txt
```

If you are using a virtual environment, activate it first.

## Running the Notebook

Open and run the notebook at `project_01/Real_Estate_Price_Prediction.ipynb` in Jupyter or JupyterLab. The notebook walks through:

- Data cleaning and preprocessing
- Exploratory data analysis and visualization
- Model training and validation
- Error fixes for current scikit-learn versions

## Notes

- The notebook was updated to remove an invalid `normalize` parameter from `LinearRegression` hyperparameter tuning, which is no longer supported in recent scikit-learn versions.
- Large binary artifacts like the model pickle file are included in `project_01/`, but can be excluded from git version control if desired.

## License

This project is provided as-is for learning and demonstration purposes.
