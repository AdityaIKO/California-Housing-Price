# Real Estate Price Prediction Model

![HOUSING](https://images.unsplash.com/photo-1589927725301-dda06a332802?q=80&w=3149&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

## Overview
This project focuses on developing a machine learning model to predict real estate prices based on historical data and current market conditions. The model aims to assist property agents and brokers in accurately estimating property prices, improving decision-making, enhancing client satisfaction, and optimizing sales processes.

--

## Project Structure
### Business Understanding
- Context: 
    - The real estate market is highly competitive, with property agents needing accurate pricing models to match clients with suitable properties.
- Problem Statement: 
    - Property agents struggle with accurate price estimation, leading to potential overpricing or underpricing, which affects sales efficiency and client trust.
- Objectives: 
    - Develop a predictive model for property prices and a client matching algorithm to improve transaction success rates.
- Success Criteria: 
    - The model should minimize errors like overprediction (leading to prolonged listing times) and underprediction (leading to underselling).

### Data Preparation
- Data Splitting: 
    - The dataset was split into training, validation, and unseen (test) data to ensure robust model evaluation.
- Feature Selection: 
    - Key features influencing property prices were selected based on prior analysis and research.
- Transformation: 
    - Log transformation was applied to the target variable to handle skewness, and features were standardized.

### Modeling
- Algorithm Used: XGBoost Regressor (XGB 1) was chosen as the final model after extensive hyperparameter tuning and comparison with other models.
- Metrics:
    - Mean Absolute Error (MAE): Focused on for its straightforward interpretation in currency units.
    - Mean Absolute Percentage Error (MAPE): Provided a percentage error to understand relative prediction accuracy.
    - Root Mean Squared Error (RMSE): Used to penalize larger errors more significantly.
- Cross-Validation: Ensured model consistency and prevented overfitting.
- Feature Importance: Identified key features like ocean_proximity and median_income as primary drivers of property prices.

### Model Evaluation
- Validation Performance:
    - MAE: 31,468.66
    - RMSE: 50,181.79
    - MAPE: 0.164405
- Unseen Data Performance:
    - MAE: 29,479.52
    - RMSE: 45,805.06
    - MAPE: 0.153654
- Business Impact
    - The model provides property agents with accurate price predictions, helping them make informed decisions and improve client trust.
    - By reducing the risk of mispricing, the model contributes to faster and more successful transactions.

--

## Deployment
### Model Deployment
- The final model was saved as california_housing_1990.pkl.
- The model can be deployed via:
    - WebApp Integration: A user-friendly web interface for property agents.
    - API Deployment: Accessible through an API for integration into existing property management systems.

### Future Work:
- Model Improvement: 
    - Continued monitoring and updating of the model based on new data and market changes.
- Business Expansion: 
    - Extending the model to include more features or adapt to different real estate markets.

--

## How To Use
### Load the Model

### Make Predictions

--

## Conclusion
This project successfully developed a robust machine learning model for predicting real estate prices. The model’s deployment in real-world applications promises to enhance the efficiency and accuracy of property transactions, ultimately benefiting both property agents and their clients.