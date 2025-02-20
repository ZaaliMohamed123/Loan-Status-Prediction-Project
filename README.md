# **Loan Status Prediction Project**

This project aims to predict the status of a loan application based on various applicant attributes using a machine learning model. The project involves data collection, preprocessing, analysis, visualization, model training, and evaluation to build an accurate predictive system.

**Steps and Methodology:**

1.	Importing Dependencies:
 *	Libraries such as numpy, pandas, seaborn, and scikit-learn are imported for data manipulation, visualization, and machine learning tasks.
2.	Data Collection:
 *	The dataset is loaded into a pandas DataFrame .
 * Basic exploration is done to understand the structure and contents of the dataset.
3.	Handling Missing Values:
 * Missing values are identified and dropped to ensure data consistency.
4.	Data Analysis and Visualization:
 *	Summary statistics and data types are checked using describe and info methods.
 *	Visualizations are created using seaborn to analyze the relationship between features like Education, Marital Status, and Loan Status.
5.	Data Preprocessing:
 *	Inconsistent data in the 'Dependents' feature is cleaned.
 *	Categorical features are label encoded to convert them into numerical values suitable for the model.
 *	Standardization is applied to numerical features .
 *	Features (X) and the target variable (Y) are separated. .
6.	HyperParameter Selection for SVC Model:
 *	A GridSearchCV is used to find the best hyperparameters for the SVC model by evaluating different combinations of parameters using cross-validation.
7.	Model Training:
 *	The dataset is split into training and test sets.
 *	An SVC model with the best parameters found in the previous step is trained on the training data.
8.	Model Evaluation:
 *	The trained model's accuracy is evaluated on both training and test data to ensure it performs well.
9.	Predictive System:
 *	A function predict_loan_status is created to predict the loan status for new input data. It preprocesses the input data, applies the trained model, and prints whether the loan is likely to be approved ('Yes') or not ('No').

