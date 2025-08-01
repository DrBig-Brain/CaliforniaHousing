# California Housing Price Prediction

This project analyzes and predicts housing prices in California using machine learning techniques.

## Project Structure

- `EDA.ipynb` — Exploratory Data Analysis notebook.
- `modeling.ipynb` — Model selection and hyperparameter tuning.
- `model.ipynb` — Model training, evaluation, and saving.
- `housing.csv` — Original dataset.
- `X.csv`, `y.csv` — Processed features and target variable.
- `model.pkl` — Saved trained model.
- `.gitignore` — Files and folders to be ignored by git.
- `readme.md` — Project documentation.
- `requirements.txt` — Python dependencies.

## Workflow

1. **Data Exploration**  
   Use `EDA.ipynb` to explore the dataset, handle missing values, and visualize features.

2. **Preprocessing**  
   - Missing values in `total_bedrooms` are imputed using the median.
   - The categorical feature `ocean_proximity` is encoded using `OrdinalEncoder`.
   - Features (`X.csv`) and target (`y.csv`) are saved for modeling.

3. **Modeling**  
   - `modeling.ipynb` explores different regressors and hyperparameters (e.g., AdaBoost, Gradient Boosting).
   - `model.ipynb` trains the final model (e.g., `GradientBoostingRegressor`), evaluates performance, and saves the model as `model.pkl`.

## Usage

1. Install dependencies:
   ```sh
   pip install -r requirements.txt