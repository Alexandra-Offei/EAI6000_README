# EAI 6000 — Fundamentals of Artificial Intelligence

**Northeastern University · Roux Institute**  
**Course:** EAI 6000 Fundamentals of Artificial Intelligence  
**Language:** Python · scikit-learn · PyTorch

---

## Overview

This course covered the foundational theory and practical implementation of machine learning algorithms, from regression through clustering. Projects used real-world datasets including housing prices, energy consumption, and smart home IoT data.

---

## Projects

### Module 1 — Multiple Linear Regression (Ames Housing Dataset)
**Dataset:** Ames, Iowa housing prices · 2,930+ records

- Built a 13-feature multiple linear regression model to predict sale prices
- Manual R² calculation from scratch (SSR regression vs naive model)
- Coefficient interpretation: Year Built, Lot Area, Garage Area, Living Area, etc.
- Feature selection using domain intuition and data dictionary reference

**Tools:** Python · scikit-learn · pandas · numpy · matplotlib

---

### Module 2 — Encoding, Scaling, Regularisation & Cross-Validation
**Dataset:** Ames Housing · 2,930 rows × 80 columns

- One-hot encoding of 40+ categorical variables
- StandardScaler normalisation
- Ridge and LASSO regularisation with GridSearchCV hyperparameter tuning
- Train/test split (80/20) with discussion of data leakage and encoding order
- Overfitting vs underfitting analysis with learning curves

**Tools:** Python · scikit-learn · pandas · numpy

---

### Module 3 — Electricity Grid Consumption Forecasting ⭐
**Dataset:** Smart building energy time series · train/test parquet files

**Target:** Predict electricity imported from grid (kW)

- Time series feature engineering: hour of day, day of week, month, lag features, rolling statistics
- Temperature, humidity, solar irradiance, and wind speed as predictors
- Models trained and compared: Linear Regression · Ridge · LASSO · Random Forest · Gradient Boosting
- Out-of-sample R² evaluation on held-out test set
- **Gradient Boosting** selected as final model for best generalisation performance

**Tools:** Python · scikit-learn · pandas · seaborn · matplotlib

---

### Module 4 — Smart Thermostat Override Classification ⭐
**Dataset:** Ecobee smart thermostat · single U.S. household · 1 year · 5-minute intervals

**Target:** Classify whether a user will override the programmed thermostat schedule

- Temporal train/test split (first 80% train, last 20% test) — respects time ordering
- Feature engineering: hour, day of week, weekend flag, month, cyclic encoding, lag features, rolling statistics
- Logistic Regression with class imbalance handling
- ROC-AUC evaluation · confusion matrix · classification report
- Analysis of which hours and days trigger most overrides

**Tools:** Python · scikit-learn · pandas · seaborn · matplotlib

---

### Module 5 — Smart Thermostat User Clustering ⭐
**Dataset:** Ecobee dataset · multiple users · hourly observations

- Aggregated hourly data to **38 per-user behavioural features**:
  - Temperature preferences (setpoints, indoor temps)
  - Comfort band (gap between heat and cool setpoints)
  - Override frequency by time of day and season
  - Energy usage patterns
- Clustering algorithms compared: **KMeans · DBSCAN · Gaussian Mixture Model**
- **PCA** for dimensionality reduction and cluster visualisation
- **Silhouette scoring** for optimal cluster number selection
- Segment profiles: energy-conscious users · comfort-maximisers · schedule-followers · irregular users

**Tools:** Python · scikit-learn · pandas · matplotlib · seaborn

---

## Skills Demonstrated

`Python` `scikit-learn` `Supervised learning` `Unsupervised learning` `Time series feature engineering` `Regularisation` `Cross-validation` `IoT data` `Energy analytics` `Clustering` `PCA` `Gradient Boosting`
