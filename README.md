# Obesity-Rate-DecisionTree

## Overview
This project demonstrates a basic Decision Tree Regressor to predict population-level obesity rates (% of adults with BMI ≥30) using proxies for food intake (low fruit/veg consumption), exercise (no leisure-time activity), and drinks (sugary intake). Built with scikit-learn and a simulated toy dataset mimicking CDC BRFSS trends. Ideal for learning tree-based regression on health data.

Key features:
- Simple dataset creation.
- Model training, prediction, and evaluation (R², RMSE).
- Bar chart visualization of actual vs. predicted rates.

Inspired by obesity research showing correlations between behaviors and rates[2][3][6]. Not for medical use—correlational only.

## Installation
1. Clone the repo:
git clone https://github.com/yourusername/Obesity-Rate-DecisionTree.git
cd Obesity-Rate-DecisionTree

2. Install dependencies:

## Usage
Run the script in Python (e.g., Jupyter Notebook). It creates a toy dataset, trains the model, evaluates, and plots.


- **Output Example**: R² ~0.951, RMSE ~2.55 (on toy data; varies with real data).
- Customize: Replace `data` with your CDC pivoted DataFrame.

## Dataset
- Toy data: 10 samples with proxies (higher % = poorer habits).
- For real use: Pivot CDC BRFSS data as shown in comments.

## Evaluation
- R²: Variance explained (higher better).
- RMSE: Prediction error (lower better).

## Limitations
- Small toy data may overfit; use larger datasets for robustness.
- Assumes regression; for classification (obese/non-obese), switch to `DecisionTreeClassifier`.

## Contributing
Fork, modify, and submit a pull request. Follow PEP 8 style.

## License
MIT License.

## Acknowledgments
- scikit-learn for modeling.
- Inspired by CDC health data analyses.
