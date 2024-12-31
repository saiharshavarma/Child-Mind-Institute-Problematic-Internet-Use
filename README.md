# Predicting Problematic Internet Use (PIU) in Adolescents

## Overview

This project focuses on predicting Problematic Internet Use (PIU) among adolescents using machine learning models. PIU, characterized by excessive internet usage leading to distress or impairment in daily functioning, has been linked to adverse mental, physical, and social outcomes. This work employs innovative methods to analyze heterogeneous tabular data and time-series accelerometer data, addressing significant data gaps and providing actionable insights.

## Objectives

- Develop a predictive framework for PIU among adolescents.
- Utilize demographic, psychological, and behavioral factors to enhance prediction accuracy.
- Compare the performance of various machine learning techniques, including traditional and deep learning models, to identify the most effective methods for heterogeneous datasets.

## Dataset

The dataset used for this study is derived from the Healthy Brain Network, encompassing:

- **Demographic variables**: Age, gender, socioeconomic indicators.
- **Behavioral patterns**: Internet usage habits, specific application usage.
- **Psychological metrics**: Anxiety, self-control, impulsivity scores.
- **Physical activity data**: Collected from ActiGraph accelerometers.
- **Target variable**: Severity Impairment Index (SII) based on PCIAT scores, categorized into None, Mild, Moderate, and Severe.

## Methodology

The project incorporates the following steps:

1. **Exploratory Data Analysis (EDA)**: Identifying patterns in internet usage, age-specific trends, and correlations with psychological and physical health metrics.
2. **Preprocessing**:
   - Handling missing values using KNN Imputation.
   - Encoding categorical data and scaling continuous variables.
   - Reducing time-series data dimensionality using LSTM autoencoders.
   - Addressing class imbalance with ensemble models.
3. **Model Development**:
   - Traditional models: Random Forest, Stacking, and Voting ensembles.
   - Gradient boosting frameworks: LightGBM, XGBoost, CatBoost.
   - Neural network models: LSTM Autoencoder, TabNet.
4. **Evaluation**: Using Quadratic Weighted Kappa (QWK) as the primary metric, reflecting ordinal relationships in SII classes.

## Results

- **Best Performance**: Voting and stacking ensemble models with gradient boosting, coupled with LSTM autoencoder-based preprocessing, achieved the highest QWK scores.
- **Key Insights**:
  - LSTM autoencoding for time-series data improves prediction accuracy significantly.
  - Traditional machine learning approaches outperformed more recent deep learning methods for this heterogeneous dataset.

## Key Findings

1. LSTM autoencoding combined with KNN imputation is highly effective for datasets with significant missing values.
2. Gradient boosting models excel in handling heterogeneous tabular data.
3. Addressing class imbalance is crucial for improving model performance on underrepresented categories.

## Conclusion

The integration of advanced preprocessing techniques and robust machine learning models enables accurate prediction of PIU among adolescents. These findings provide a scalable framework for early intervention and decision-making, highlighting the practicality of combining deep learning and traditional methods for real-world datasets.

### Future Work

- Incorporate additional data sources for more comprehensive modeling.
- Optimize deep learning architectures like TabNet for better results.
- Address overfitting in ensemble models through advanced regularization techniques.

---
