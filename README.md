## Project Overview 
Crime prediction is a challenging task due to complex spatial–temporal patterns, missing data, and class imbalance.
This project explores different supervised learning approaches to forecast where crime is most likely to occur next.

The workflow includes:

- Data cleaning and preprocessing
- Feature encoding and selection
- Model training using:
- Decision Trees
- Random Forests
- Neural Networks with Cross-Validation
- Evaluation using standard classification metrics
- Interpretation and comparison of model performance


## Dataset :

- Crime type
- Date and time of incident
- Geographic coordinates (Lat/Lon)
- Area and reporting district
- Victim demographics
- Additional situational variables

Note: Dataset is not included in this repository due to size and privacy constraints.

A variety of data preprocessing steps were applied to prepare the data for modeling:

1. Handling Missing Values
- Numerical features were imputed with mean values.
- Categorical missing values handled appropriately per feature.

3. Categorical Encoding
- Applied One-Hot Encoding to convert categorical features into numerical representations.

3. Feature Selection
   - Removed irrelevant or redundant features.
   - Evaluated feature importance using tree-based methods and correlation analysis.

5. Addressing Class Imbalance
  -Class distribution was analyzed.
  -Appropriate metrics (precision/recall/F1 per class) used to ensure minority-class fairness.


## Machine Learning Models

Several models were trained and evaluated to compare predictive performance. These models are : Decision Tree, Random Forest and Neural Network with Cross Validation.

## Model Evaluation

Models were evaluated using:
- Accuracy
- Precision, Recall, F1-Score per class
- Confusion Matrix
- Cross-Validation Scores
Special emphasis was placed on minority-class performance (less frequent crime hotspot labels).

## Results 

A summary of findings:

- Random Forest generally produced the best overall performance.
- Decision Trees served as a strong, interpretable baseline.
- Neural Networks benefited from cross-validation but were sensitive to preprocessing and class imbalance.
- Feature importance revealed key predictors such as geographic location, time-based variables, and certain crime categories.

## Future improvemnts :
 - Different prerprocessing techniques and models could be tried.
 - For time series data we could use time temporal CNN

