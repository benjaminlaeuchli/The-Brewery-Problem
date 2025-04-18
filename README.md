![Description of image](https://github.com/benjaminlaeuchli/The-Brewery-Problem/blob/main/9786c369-ecd3-4fe7-bcf6-eec26d1fec8b.png?raw=true)

## Beer Rating Prediction with Machine Learning

This project focuses on building a predictive machine learning pipeline to estimate beer ratings based on features such as alcohol content (ABV), bitterness (IBU), brand awareness, and beer style. It includes data preprocessing, imputation of missing values, model training, evaluation, and prediction.

**Project Goals**
- Clean and preprocess a messy dataset containing beer attributes.
- Explore multiple approaches to handle missing data, including KNN imputation.
- Train machine learning models to predict the Rating of beers.
- Use the model to predict ratings for unseen test and target datasets.

**Dataset Overview**
The dataset includes beer attributes such as:

ABV: Alcohol by volume
IBU: International Bitterness Units
Rating: Consumer rating score
Brand Awareness: A measure of how well-known the brand is
Style_ale, Style_lager, Style_hybrid: One-hot encoded beer styles

**Datasets used:**

df_train: Training data with some rows having all values concatenated into a single column (requiring parsing)
df_test: Test data in a similar format
df_aim: Target data for final prediction

**Data Preprocessing**
Parsing and splitting columns: Rows with semicolon-separated values are split into individual features.
Locale-aware float parsing: Handles comma vs. dot decimal formats.

**Missing value handling:**

Rows with clean numerical entries are left unchanged.
Rows with merged strings are split and converted.

**KNN Imputation:** Applied to numerical features to fill in remaining missing values.

**Model Training**
- Machine Learning models explored (Lineaer Regression, Ridge Regression, Lasso regression, RANSAC)
- Grid search and parameter tuning for RANSAC model
- Visualize feature importance 

**Prediction & Output**
Predictions are made on cleaned df_test and df_aim datasets using the trained model.

Final predicted ratings are displayed or exported.
