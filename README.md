#  Adult Census Income Level Prediction
## Integrated ML Pipeline: Data Engineering (R) & Modeling (KNIME) | Data Science Master's Degree
This project implements a comprehensive machine learning pipeline to predict whether an individual's income exceeds $50,000/year based on census data. By integrating R for high-precision data cleaning and KNIME for visual workflow orchestration, the project explores the impact of various data-balancing techniques across seven distinct classification algorithms.

## 1. Data Pre-processing (R Integration)
 - Initial data refinement was performed using R to ensure a clean, standardized foundation for modeling:

- Handling Missing Values: Identification of incomplete records (often marked as "?" in census data) and application of imputation or removal strategies.

- Feature Transformation: Conversion of categorical variables into numerical formats and scaling of continuous features (e.g., age, hours-per-week).

- Data Partitioning: Splitting the dataset into dedicated training and testing sets to ensure unbiased evaluation.

## 2. Addressing Class Imbalance
The "Adult Census" dataset is notoriously imbalanced, with significantly fewer individuals in the >50K category. This project evaluates three strategies to mitigate this bias:

- Equal Size Sampling (ESS): Balancing the classes by randomly under-sampling the majority class.

=- SMOTE (Synthetic Minority Over-sampling Technique): Generating synthetic training examples for the minority class.

- Cost-Sensitive Learning: Adjusting the model's cost function to penalize misclassifications of the minority class more heavily.

## 3. Machine Learning Models
The predictive core involves seven different algorithms implemented in KNIME, covering tree-based, probabilistic, and connectionist approaches:

- Decision Trees & Ensembles: J48 (C4.5), Random Forest (RF), and NBTree (Naive Bayes Tree).

- Linear & Kernel Models: Logistic Regression and Support Vector Machines (SVM).

- Probabilistic & Neural: BayesNet and Multi-Layer Perceptron (MLP).

## 4. Evaluation Framework
The models were rigorously assessed through a multi-dimensional validation matrix:

- Methodology: Comparative analysis between the Holdout Method and K-Fold Cross-Validation.

- Feature Selection: Optimization of the feature space to improve model interpretability and reduce noise.

- Performance Metrics: Detailed assessment of Accuracy, Precision, Recall, and F1-Score, specifically focusing on the minority class performance.

Assessment Scenarios
