# Obesity Rate Prediction with Decision Tree

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Yashas7206988696/Obesity-Rate-Prediction-with-Decision-Tree/blob/main/code.ipynb)

## Project Overview

This project demonstrates the application of Decision Tree Regression for predicting obesity rates at the population level. The model predicts the percentage of adults with BMI ≥30 using behavioral health indicators as predictive features. This implementation serves as an educational tool for understanding tree-based regression algorithms in the context of public health data analysis.

## Decision Tree Regressor Methodology

### Algorithm Overview
The Decision Tree Regressor is a non-parametric supervised learning method used for regression tasks. It creates a model that predicts target values by learning simple decision rules inferred from data features.

### Key Characteristics:
- **Non-linear relationships**: Captures complex patterns without assuming linear relationships
- **Feature importance**: Provides insights into which variables contribute most to predictions
- **Interpretability**: Easy to visualize and understand the decision-making process
- **No assumptions**: Does not require assumptions about data distribution

### Implementation Details:
- Uses scikit-learn's `DecisionTreeRegressor`
- Employs standard regression evaluation metrics (R², RMSE)
- Includes visualization of actual vs predicted values

## Dataset

### Current Implementation:
- **Size**: 10 samples (toy dataset for demonstration)
- **Features**: 3 behavioral health indicators
  - Low fruit/vegetable consumption percentage
  - No leisure-time physical activity percentage  
  - High sugary drink intake percentage
- **Target**: Obesity rate (% of adults with BMI ≥30)

### Data Structure:
The dataset simulates real-world health survey data with correlational patterns between lifestyle behaviors and obesity rates, inspired by CDC BRFSS (Behavioral Risk Factor Surveillance System) trends.

### Real Data Integration:
For production use, the code includes comments showing how to integrate actual CDC BRFSS pivoted data to replace the toy dataset.

## Code Features

### Core Functionality:
1. **Data Generation**: Creates simulated health behavior dataset
2. **Model Training**: Implements Decision Tree Regressor with scikit-learn
3. **Model Evaluation**: 
   - R² score (coefficient of determination)
   - RMSE (Root Mean Square Error)
4. **Visualization**: Bar chart comparison of actual vs predicted obesity rates
5. **Extensibility**: Framework ready for real CDC data integration

### Key Libraries Used:
- `pandas`: Data manipulation and analysis
- `numpy`: Numerical computations
- `scikit-learn`: Machine learning algorithms and evaluation
- `matplotlib`: Data visualization

## Requirements

```python
pandas>=1.3.0
numpy>=1.21.0
scikit-learn>=1.0.0
matplotlib>=3.4.0
```

## Installation & Usage

### Option 1: Google Colab (Recommended)
**🚀 [Open in Google Colab](https://colab.research.google.com/github/Yashas7206988696/Obesity-Rate-Prediction-with-Decision-Tree/blob/main/code.ipynb)** - Run instantly in your browser!

### Option 2: Local Installation
1. Clone the repository:
```bash
git clone https://github.com/Yashas7206988696/Obesity-Rate-Prediction-with-Decision-Tree.git
cd Obesity-Rate-Prediction-with-Decision-Tree
```

2. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib
```

3. Run the Jupyter notebook:
```bash
jupyter notebook code.ipynb
```

## Model Performance

### Expected Results (Toy Dataset):
- **R² Score**: ~0.951 (95.1% variance explained)
- **RMSE**: ~2.55 (average prediction error)

*Note: Performance metrics will vary with real-world data and may require hyperparameter tuning for optimal results.*

## Colab Integration Highlights

### 🌟 **Quick Start with Colab**
- **Zero Setup**: No local installation required
- **GPU/TPU Access**: Leverage Google's computational resources
- **Easy Sharing**: Share results with a simple link
- **Pre-installed Libraries**: All required packages ready to use

### 📊 **Interactive Features in Colab**:
- Real-time code execution and visualization
- Inline plotting with matplotlib
- Easy data upload and download capabilities
- Seamless integration with Google Drive

**💡 Pro Tip**: Click the Colab badge above to start experimenting immediately!

## Model Evaluation Metrics

### R² (Coefficient of Determination)
- **Range**: 0 to 1 (higher is better)
- **Interpretation**: Proportion of variance in obesity rates explained by the model
- **Good Performance**: R² > 0.8

### RMSE (Root Mean Square Error)
- **Units**: Same as target variable (percentage points)
- **Interpretation**: Average prediction error
- **Good Performance**: Lower RMSE indicates better accuracy

## Limitations & Considerations

### Current Limitations:
- **Small Dataset**: Toy data may lead to overfitting
- **Simplified Features**: Real obesity factors are more complex
- **Correlation vs Causation**: Model shows associations, not causal relationships

### Recommendations for Production Use:
- Use larger, more diverse datasets (CDC BRFSS, WHO data)
- Include additional features (demographics, socioeconomic factors)
- Implement cross-validation for robust evaluation
- Consider ensemble methods for improved accuracy

## Future Enhancements

- [ ] Integration with real CDC BRFSS data
- [ ] Feature engineering for improved predictions
- [ ] Hyperparameter optimization
- [ ] Model comparison (Random Forest, XGBoost)
- [ ] Interactive web dashboard
- [ ] Classification variant for obesity categories

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit changes (`git commit -am 'Add improvement'`)
4. Push to branch (`git push origin feature/improvement`)
5. Create a Pull Request

Please follow PEP 8 style guidelines for Python code.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **scikit-learn**: For providing excellent machine learning tools
- **CDC BRFSS**: Inspiration from real-world health surveillance data
- **Google Colab**: For enabling accessible machine learning education
- **Open Source Community**: For continuous support and improvements

## Citation

If you use this code in your research or projects, please cite:

```bibtex
@software{obesity_decision_tree_2024,
  title={Obesity Rate Prediction with Decision Tree},
  author={Yashas7206988696},
  year={2024},
  url={https://github.com/Yashas7206988696/Obesity-Rate-Prediction-with-Decision-Tree}
}
```

---

**⚠️ Disclaimer**: This project is for educational and research purposes only. It is not intended for medical diagnosis or treatment decisions. Always consult healthcare professionals for medical advice.
