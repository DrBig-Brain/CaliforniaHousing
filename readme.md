# California Housing Price Prediction

This project analyzes and predicts housing prices in California using machine learning techniques.

## Project Structure

- `EDA.ipynb` - Exploratory Data Analysis notebook.
- `modeling.ipynb` - Model selection and hyperparameter tuning.
- `model.ipynb` - Model training, evaluation, and saving.
- `housing.csv` - Original dataset.
- `X.csv`, `y.csv` - Processed features and target variable.
- `model.pkl` - Saved trained model.
- `.gitignore` - Files and folders to be ignored by git.
- `readme.md` - Project documentation.

## Workflow

1. **Data Exploration**:  
   Use `EDA.ipynb` to explore the dataset, handle missing values, and visualize features.

2. **Preprocessing**:  
   - Missing values in `total_bedrooms` are imputed using the median.
   - The categorical feature `ocean_proximity` is encoded using `OrdinalEncoder`.
   - Features (`X.csv`) and target (`y.csv`) are saved for modeling.

3. **Modeling**:  
   - `modeling.ipynb` explores different regressors and hyperparameters (e.g., AdaBoost, Gradient Boosting).
   - `model.ipynb` trains the final model (e.g., `GradientBoostingRegressor`), evaluates performance, and saves the model as `model.pkl`.

## Usage

1. Clone the repository and install dependencies (e.g., pandas, scikit-learn, matplotlib, seaborn).
2. Run the notebooks in order:
   - `EDA.ipynb`
   - `modeling.ipynb`
   - `model.ipynb`
3. Use the saved `model.pkl` for predictions on new data.

## Requirements

- Python 3.6+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## References

- [California Housing Dataset - Kaggle](https://www.kaggle.com/datasets/camnugent/california-housing-prices)
