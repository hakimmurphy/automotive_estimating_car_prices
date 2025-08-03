# Automotive Estimating Car Prices

Estimate used car prices for a local dealership using machine learning and feature engineering.

## Project Structure

```
Automotive_Estimating_Car_Prices.ipynb  # Main Jupyter notebook
cars.csv                                # Dataset
requirements.txt                        # Python dependencies
best_car_price_model.pkl                # Saved trained model
```

## Features

- Data cleaning and preprocessing
- Feature engineering (car age, brand premium/discount, segment value, etc.)
- Exploratory data analysis (EDA) with visualizations
- Predictive Power Score (PPS) and correlation analysis
- Model training and evaluation (Linear, Ridge, Lasso, Decision Tree, Random Forest, Gradient Boosting, XGBoost)
- Hyperparameter tuning with GridSearchCV
- Model saving for deployment

## Getting Started

1. **Clone the repository and navigate to the project folder.**

2. **Install dependencies:**
   ```
   pip install -r requirements.txt
   ```

3. **Run the notebook:**
   Open `Automotive_Estimating_Car_Prices.ipynb` in Jupyter or VS Code and run the cells in order.

4. **Dataset:**
   - The notebook expects a `cars.csv` file in the project root.

## Usage

- The notebook walks through the full workflow: loading data, cleaning, feature engineering, EDA, model training, evaluation, and saving the best model.
- The trained model is saved as `best_car_price_model.pkl` and can be loaded for future predictions.

## Requirements

See [requirements.txt](requirements.txt).

## Model Deployment

To load the trained model in Python:

```python
import pickle

with open('best_car_price_model.pkl', 'rb') as f:
    model = pickle.load(f)
# model.predict(...)
```

## Author

Hakim Murphy
