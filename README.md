# SHAP-Driven-Rare-Event-Detection-in-Multivariate-Industrial-Time-Series
This project provides a beginner-friendly yet research-grade workflow for detecting and explaining rare anomalies in multivariate industrial time-series data.
SHAP-Driven Rare-Event Detection in Multivariate Industrial Time Series

Interpretable Fault Analytics Using XGBoost + Shapley Values

This project provides a beginner-friendly yet research-grade workflow for detecting and explaining rare anomalies in multivariate industrial time-series data.
It demonstrates how to convert raw sensor streams into a supervised learning format, train an imbalance-aware classifier, and generate interpretable SHAP attributions suitable for engineering diagnostics (e.g., Honeywell DCS/EPKS environments).

 **Project Overview**

Industrial systems generate high-dimensional sensor data where faults are extremely rare, nonlinear, and temporally dependent. Traditional anomaly detection often lacks transparency.
This project bridges that gap by pairing XGBoost with SHAP (TreeExplainer) to provide:

Exact Shapley-value feature attributions

Sensor-level and lag-level interpretability

Local (per-event) explanations

Global importance across the full monitoring horizon

The methodology emphasizes clarity, reproducibility, and engineering usability.

**Key Features**

Multivariate time-series ingestion & preprocessing
Clean loading, timestamp parsing, and quality checks for industrial sensor signals.

Temporal feature engineering
Sliding-window lag construction enabling supervised learning from sequential data.

Imbalance-aware model training
XGBoost with scale_pos_weight to learn subtle fault signatures under extreme rarity.

Robust evaluation metrics
Precision, recall, F1, and ROC–AUC for meaningful rare-event performance assessment.

Global SHAP analysis
Summary plots and bar charts highlighting the most influential sensors/lags.

Sensor-level SHAP aggregation
Converts hundreds of lag features into simple, engineering-interpretable rankings.

