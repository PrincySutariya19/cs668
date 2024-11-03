# Supply Chain Optimization for Health Commodity Shipment and Pricing

### Princy Sutariya  
## Objective  
To use predictive modeling for optimizing costs and efficiency in the supply chain of HIV-related health commodities.

## Motivation  
This project focuses on improving the reliability and cost-effectiveness of health commodity distribution in developing countries to ensure affordable and timely access to essential products for combating HIV.

## Research Questions  
1. How can supply chain costs be minimized for HIV-related health commodities?
2. What are the primary causes of delivery delays, and how can they be predicted?
3. How can pricing be optimized across regions for better cost efficiency?

## Literature Review  
The literature emphasizes the need for accurate demand forecasting, efficient inventory management, and transparency in supply chains to enhance access to critical health products. This project leverages machine learning (e.g., XGBoost, RandomForest) for predicting shipment costs and delivery times. SHAP is used for model explainability, and Streamlit for real-time forecasting, promoting a data-driven, equitable approach to global health supply chains.

## Dataset Overview  
The dataset comprises 10,324 rows and 33 columns covering various aspects of supply chain logistics for HIV commodities in developing countries. Key features include:
- **Cost Details** (freight, insurance, unit price)
- **Logistics Management** (vendor, shipment mode, weight)

**Dataset Link:** [Supply Chain Shipment Pricing Data](https://catalog.data.gov/dataset/supply-chain-shipment-pricing-data-07d29)

## EDA & Methodology  
1. **Data Preprocessing:** Handled missing values, standardized features, and engineered new metrics (e.g., cost per unit weight).
2. **Modeling Approach:**
   - **Freight Cost Prediction:** Implemented using XGBoost (with potential plans to explore linear regression).
3. **Optimization & Experimentation:** Optimized model parameters through Grid and Random Search. Implemented cost optimization via Linear and Mixed-Integer Linear Programming.

## Model Results & Evaluation  
**Freight Cost Prediction:**

- **Models Used:** XGBoost Regressor
- **Evaluation Metrics:** Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² Score.
- **Results:**
   - XGBoost: MAE = 488.94, RMSE = 1675.92, R² = 0.988

## Next Steps  
1. **Model Tuning:** Experiment with additional models (e.g., Gradient Boosting, Neural Networks) and advanced hyperparameter tuning (e.g., Bayesian Optimization).
2. **Delay Prediction Expansion:** Expand models to predict shipment delays using additional features like historical delays, vendor performance, and seasonal factors.
