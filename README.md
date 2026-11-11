# Diabetes Data Analysis and Preprocessing

This project contains a notebook-based exploratory data analysis (EDA) and preprocessing workflow for a diabetes dataset. The goal is to understand the dataset, inspect feature distributions, detect outliers, analyze relationships between variables, and prepare the data for further machine learning tasks such as classification modeling.

## Project Files

- `diabetes.ipynb` — Jupyter notebook with the full analysis workflow
- `diabetes.csv.xls` — dataset used for the study

## Dataset Overview

The dataset includes medical and health-related features used to study diabetes risk. The target column, `Outcome`, is a binary label indicating whether a patient is diabetic or not.

Each row represents a patient record, and the features include variables such as:

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- Outcome

## Objectives

- Load and inspect the dataset
- Check the data shape and column types
- Identify missing values and data quality issues
- Visualize feature distributions using boxplots
- Detect extreme outliers using the IQR method
- Explore relationships among variables using correlation analysis
- Review class balance in the target variable
- Apply feature scaling using Min-Max and Standard scaling techniques

## Tools and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

## Workflow Summary

1. Import the dataset with Pandas.
2. Inspect data structure and summary information.
3. Check for null values and confirm dataset dimensions.
4. Plot boxplots for all numerical columns to study distribution and outliers.
5. Remove outliers from the `Insulin` feature using the IQR rule.
6. Compute a correlation matrix and visualize it with a heatmap.
7. Review the relationship between variables and the target column.
8. Plot the outcome distribution to examine class balance.
9. Split features and target for model-ready preparation.
10. Apply Min-Max scaling and Standard scaling to the independent variables.

## Key Observations

- The dataset contains no missing values, based on the null-check step.
- Outlier filtering is applied to the `Insulin` feature to reduce extreme values.
- Correlation analysis helps reveal which variables are most strongly associated with the outcome.
- Feature scaling is used to normalize input values before model training, which can improve machine learning performance.

## How to Run

Open the notebook in Jupyter Notebook or VS Code with a Python kernel and run the cells in order.

```bash
jupyter notebook diabetes.ipynb
```

## Notes

This project focuses on data exploration and feature preprocessing. It is a strong foundation for the next steps in a machine learning pipeline, such as:

- train/test splitting
- model selection
- evaluation using accuracy, precision, recall, and F1-score
- hyperparameter tuning

## Future Improvements

- Build a classification model such as Logistic Regression, Random Forest, or SVM
- Evaluate the model using cross-validation and confusion matrix
- Compare performance before and after scaling
- Save the trained model and preprocessing pipeline for deployment

## License

This project is intended for educational and learning purposes.
