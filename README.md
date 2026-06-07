# Xgboost-model-actuarial-pricing
Machine learning model for actuarial pricing
# French Motor Third-Party Liability Insurance Premium Modeling

This repository contains a Python implementation for processing and analyzing French Motor Third-Party Liability insurance risk datasets (`freMTPL2freq` and `freMTPL2sev`). The script pipelines data cleaning, feature engineering, and frequency/severity preparation for advanced risk modeling with XGBoost.

## Project Overview
This provides an end-to-end, practical implementation of an actuarial risk modeling pipeline. The project bridges the gap between raw insurance data and deployment by executing five distinct phases:

1. **Data Extraction**: Dual-source data ingestion pulling historical frequency data from local `.arff` files and severity profiles directly via the scikit-learn OpenML API.
2. **Data Manipulation & Processing**: Comprehensive data cleaning, feature engineering (quantile binning), outlier capping, and deterministic alignment of policy exposures with claim amounts.
3. **Model Building**: Constructing and training a specialized XGBoost machine learning model optimized to handle highly skewed insurance claim distributions.
4. **Model Testing**: Evaluating model performance using domain-specific metrics like Mean Tweedie Deviance to validate prediction accuracy on unseen test data.
5. **Risk Rate Chart Development**: Transforming raw model outputs into a practical risk rate chart, allowing underwriters and business systems to easily look up policy risk premiums based on driver and vehicle profiles.
