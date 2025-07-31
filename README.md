# rirs-ai-saturation-model
ai model forecasting rental inflation risk score (rirs) using airbnb saturation data

🚀 Overview
Built a supervised Gradient Boosting Regressor pipeline to predict a novel Rental Inflation Risk Score (RIRS), quantifying how short-term rental saturation (via Airbnb) drives long-term rent inflation and displacement.

🛠️ Technical Highlights

1. Feature Engineering: Engineered occupancy proxies, host-portfolio flags, normalized price/availability, and composite risk labels.
2. Data Prep & Pipeline: Applied robust imputation, median-based missing-value replacement, one-hot encoding, and StandardScaler within a scikit-learn ColumnTransformer.
3. Modeling & Validation: Trained & evaluated with k-fold cross-validation, monitored RMSE & R², and compared baseline LinearRegression vs. GradientBoostingRegressor.
4. Risk Modeling: Implemented Quantile Regression (α=0.05/0.95) to generate 90% prediction intervals—critical for uncertainty quantification in finance.
5. Explainability: Used SHAP (SHapley Additive exPlanations) to dissect feature contributions at the instance level, enhancing model transparency.
6. Geospatial Analytics: Visualized RIRS on a choropleth scatter plot by latitude/longitude, enabling spatial risk mapping for portfolio optimization.
7. Advanced Insights: Plotted Estimated Revenue vs. RIRS for risk–return tradeoffs and segmented host types (Single vs. Small Portfolio vs. Institutional) to uncover scale-driven inflation effects.

💡 Business Impact

1. For REITs & Hedge Funds: A powerful tool to incorporate risk-adjusted return forecasting into location-based allocation strategies.
2. For STR Platforms: Actionable insights to optimize supply-side onboarding, balance revenue growth vs. community impact, and inform dynamic pricing strategies.
3. For Urban Policy Makers: Early-warning system to identify gentrification hotspots, support data-backed policy interventions, and model housing affordability scenarios.
