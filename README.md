---

# Predictive Maintenance using Machine Learning

This Jupyter Notebook contains a Python script for predictive maintenance using machine learning. The analysis uses the "predictive_maintenance.csv" dataset and covers data preprocessing, model building, and performance evaluation to predict the type of failures in a manufacturing process.

## Dataset

The dataset includes information about various parameters in a manufacturing process, such as air temperature, process temperature, rotational speed, torque, tool wear, and more. The primary goal is to predict the type of failures that may occur during the process.

### Data Preprocessing

- Data Cleaning: The notebook handles missing values and converts temperature measurements from Kelvin to Celsius.
- Feature Engineering: A new feature, "Temperature difference [°C]," is created to capture the temperature variation.
- Label Encoding: Categorical variables like "Type" and "Failure Type" are encoded for model training.

### Model Building

- Logistic Regression: A logistic regression model is trained to predict failure types.
- Decision Tree Classifier: A decision tree classifier is used with a maximum depth of 3.
- Random Forest Classifier: A random forest classifier with 50 estimators is trained.
- Support Vector Classifier (SVC): A linear kernel SVC is also trained for comparison.

### Model Evaluation

- The notebook calculates and displays the accuracy scores for each model on both the training and testing datasets.
- Model performance is evaluated using appropriate metrics, including accuracy and confusion matrices.

## Usage

You can run this Jupyter Notebook in a Python environment (e.g., Jupyter Notebook or JupyterLab) to perform predictive maintenance analysis on your manufacturing process dataset. Ensure you have the required libraries installed, as mentioned in the notebook.

## Dependencies

This notebook relies on the following Python libraries:

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

You can install these libraries using pip:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---
