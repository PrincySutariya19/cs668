# Supply Chain Optimization for Health Commodity Shipment and Pricing

### Princy Sutariya  
## Objective  
To leverage predictive modeling to optimize costs and improve efficiency in the supply chain for HIV-related health commodities.

## Motivation  
This project aims to enhance the reliability and cost-effectiveness of health commodity distribution in developing countries. By doing so, it ensures affordable and timely access to essential products needed to combat HIV, bridging gaps in healthcare delivery systems.

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
1. **Data Preprocessing:** Handled missing values, Standardized and scaled numerical features, Engineered new features (e.g., total cost, cost per unit weight)
2. **Modeling Approach:**
   - **Freight Cost Prediction:** Implemented using XGBoost (with potential plans to explore linear regression).
3. **Optimization & Experimentation:** Optimized model parameters through Grid and Random Search. Implemented cost optimization via Linear and Mixed-Integer Linear Programming.

## Model Results & Evaluation  
**Freight Cost Prediction:**

- **Models Used:** XGBoost & Linear Regression
- **Evaluation Metrics:** Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² Score.
- **Results:**
   - XGBoost:RMSE = 943.644, R² = 0.996
   - Linear Regression: RMSE= 300.78, R² = 0.9996

## Conclusion  
Both models performed exceptionally well, but XGBoost's robustness in handling non-linear relationships makes it ideal for complex datasets, while Linear Regression provides a simpler, interpretable approach with slightly better accuracy in this dataset.
