# house-price-prediction-ml

## Project Objective
Predict house sale prices using structured housing data from the Kaggle "House Prices: Advanced Regression Techniques" competition.

## Dataset Used
- `data/raw/train.csv`
- 81 columns and 1460 rows
- Target: `SalePrice`
- Key features: `GrLivArea`, `BedroomAbvGr`, `Neighborhood`, `OverallQual`, `YearBuilt`, `GarageCars`, `TotalBsmtSF`, `FullBath`

## Models Applied
- Gradient Boosting Regressor
- XGBoost Regression
- Ridge Regression for baseline comparison

## Key Results and Findings
- Data cleaning handles missing values, outliers, and categorical encoding.
- Engineered features include total square footage, house age, and binary indicators for garage/basement support.
- Model performance is evaluated with MAE, RMSE, and R².
- The production inference function supports neighborhood-level predictions and returns a price estimate with a confidence interval.

## Repository Structure
- `data/raw/` — original dataset
- `data/processed/` — cleaned data outputs
- `models/` — saved trained models
- `outputs/figures/` — visualization artifacts
- `hose-price.ipynb` — main notebook workflow

## Notes
- Ensure `data/raw/train.csv` is downloaded from Kaggle and available before running the notebook.
