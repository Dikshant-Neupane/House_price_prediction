# House Price Prediction

This project predicts house sale prices using machine learning models trained on tabular housing data.

## Project Overview

The notebook in this repository performs:
- Data loading and train/test combination for preprocessing
- Missing value handling for numeric and categorical features
- Categorical encoding using one-hot encoding
- Model training and comparison
- Prediction quality check using Mean Squared Error (MSE)

## Repository Structure

```text
House_price_prediction/
├── Data/
│   ├── train.csv
│   ├── test.csv
│   ├── sample_submission.csv
│   └── data_description.txt
└── Notebook/
    └── advanced_regression.ipynb
```

## Models Used

- Linear Regression
- XGBoost Regressor
- Random Forest Regressor

## Tech Stack

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- scikit-learn
- XGBoost

## How to Run

1. Clone this repository.
2. Install dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
   ```

3. Open the notebook:

   ```bash
   jupyter notebook Notebook/advanced_regression.ipynb
   ```

4. Run all cells in order.

## Input and Output

- **Input:** `Data/train.csv` and `Data/test.csv`
- **Output:** Model performance (MSE) in notebook cells and predicted-vs-actual plot

## Notes

- The notebook preprocesses train and test data together for consistent feature engineering.
- Missing values are handled with mode/mean imputation depending on feature type.

## Future Improvements

- Add a reproducible training script (`.py`) outside the notebook
- Add cross-validation and hyperparameter tuning
- Save trained model artifacts
- Generate a final submission CSV automatically
