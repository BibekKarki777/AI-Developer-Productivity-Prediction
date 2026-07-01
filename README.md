# AI Developer Productivity Prediction

A machine learning classification project developed using **Python** and **Jupyter Notebook** to predict whether an AI developer will successfully complete a task based on productivity-related factors.

## About the Project

This project predicts developer task success using features such as coding hours, coffee intake, distractions, sleep hours, commits, bugs reported, AI tool usage hours, and cognitive load.

The project includes data loading, data inspection, missing value checking, duplicate checking, exploratory data analysis, outlier removal, feature scaling, Logistic Regression model training, model evaluation, confusion matrix visualization, actual vs predicted comparison, and model saving using Joblib.

## Problem Statement

Developer productivity can be affected by many factors, including focus time, distractions, sleep, workload, AI tool usage, caffeine intake, and cognitive load.

This project uses machine learning to predict whether a developer is likely to complete a task successfully based on these productivity-related features.

## Dataset

The dataset file used in this project is:

```text
ai_dev_productivity.csv
```

The dataset contains **500 records** and **9 columns**.

## Dataset Features

### Input Features

- `hours_coding` - Total focused hours spent on software development work
- `coffee_intake_mg` - Daily caffeine intake in milligrams
- `distractions` - Number of distractions such as meetings or notifications
- `sleep_hours` - Number of hours slept the previous night
- `commits` - Number of code commits pushed during the day
- `bugs_reported` - Number of bugs reported in code written that day
- `ai_usage_hours` - Number of hours spent using AI tools such as ChatGPT or Copilot
- `cognitive_load` - Self-reported mental strain on a scale of 1 to 10

### Target Variable

- `task_success` - Indicates whether the developer successfully completed the task

Target values:

```text
1 = Task successful
0 = Task unsuccessful
```

## Features of the Project

- Loads dataset using Pandas
- Checks dataset shape, information, and summary statistics
- Checks missing values
- Checks duplicate values
- Performs correlation analysis
- Visualizes feature distributions using histograms
- Visualizes outliers using boxplots
- Removes outliers using the IQR method
- Splits data into training and testing sets
- Scales features using StandardScaler
- Trains a Logistic Regression model
- Evaluates model using accuracy, confusion matrix, and classification report
- Visualizes confusion matrix
- Compares actual and predicted values
- Saves trained model pipeline using Joblib
- Allows user input for task success prediction

## Machine Learning Model

The project uses:

- Logistic Regression

The model is trained to classify whether the task will be successful or unsuccessful.

## Evaluation Metrics

The model is evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report
- Precision
- Recall
- F1-score

## Tech Stack

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib


## Model Saving

The trained model is saved as:

```text
ai_task_success_model.pkl
```

The saved model pipeline includes:

- StandardScaler
- Logistic Regression classifier

This allows the model to be reused for future predictions.

## Example User Input

The notebook allows users to enter values such as:

```text
hours_coding
coffee_intake_mg
distractions
sleep_hours
commits
bugs_reported
ai_usage_hours
cognitive_load
```

The model then predicts whether the developer will successfully complete the task.

## Author

**Bibek Karki**

## License

This project is created for academic and learning purposes.
