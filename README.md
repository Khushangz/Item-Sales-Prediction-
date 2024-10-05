
# Item-Sales-Prediction

Predicting item sales using feature selection and hyperparameter tuning to optimize model performance.

## Project Overview

This project aims to accurately predict item sales by identifying key features in the dataset and fine-tuning model parameters for improved accuracy. Using `ExtraTreesRegressor`, we leverage tree-based feature selection and perform hyperparameter tuning with `GridSearchCV` to build a robust model.

## Dataset

The dataset used for this project is preprocessed into a pandas DataFrame and encoded for model training. Features (X) and target variables (y) are split, with 80% used for training and 20% for testing.

## Key Steps

1. **Data Preprocessing**: 
   - Load and preprocess data to encode categorical values.
   - Split the dataset into training and test sets for model validation.

2. **Feature Selection**:
   - Apply feature importance extraction using `ExtraTreesRegressor` to identify the most impactful features for the prediction model.

3. **Hyperparameter Tuning**:
   - Define a parameter grid for tuning.
   - Use `GridSearchCV` with cross-validation to identify the optimal parameters for `ExtraTreesRegressor`.

4. **Model Evaluation**:
   - Evaluate the model using Root Mean Squared Error (RMSE) and R² Score, printing the best parameters and model performance metrics.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Item-Sales-Prediction.git
   cd Item-Sales-Prediction
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

## Usage

1. **Data Loading**: Ensure data is preprocessed and ready for training.
2. **Run the Notebook**: Execute the cells in sequence to preprocess, tune, and evaluate the model.
3. **Configure Parameters**: Modify `param_grid` to experiment with different hyperparameters.
4. **View Output**: The notebook displays the best hyperparameters and performance metrics (RMSE and R²).

## Results

The final model achieves:
- **Best Parameters**: Optimal parameters from `GridSearchCV` for `ExtraTreesRegressor`.
- **Performance Metrics**: RMSE and R² Score, with R² close to 1 indicating a better fit.

## Future Enhancements

- **Automated Feature Selection**: Add algorithms like RFE for dynamic feature selection.
- **Additional Model Comparisons**: Try models like `RandomForestRegressor` or `GradientBoostingRegressor`.
- **Scalability**: Utilize distributed frameworks (e.g., `Dask`) for large datasets.


