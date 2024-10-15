# Employee Attrition Prediction App: End-to-End ML Project

## Project Overview
This end-to-end machine learning project aims to predict employee attrition using Random forest classifier model based on HR data. We've developed a complete pipeline from data analysis to model deployment, culminating in a Gradio app for easy visualization and prediction.

![image](https://github.com/user-attachments/assets/50211152-5022-4984-9a42-721f52117297)

## Dataset Description
The Employee Attrition dataset contains various features related to employee characteristics, work patterns, and company-related factors. This dataset is designed to analyze and predict employee attrition within an organization.

### Features
The dataset includes the following features:

- satisfaction_level: Employee's reported level of job satisfaction
- last_evaluation: Score of the employee's last performance evaluation
- number_project: Number of projects the employee is involved in
- average_monthly_hours: Average number of hours the employee works per month
- time_spend_company: Number of years the employee has spent in the company
- work_accident: Whether the employee has had a work accident (1) or not (0)
- left: Target variable indicating whether the employee has left the company (1) or not (0)
- promotion_last_5years: Whether the employee has been promoted in the last 5 years (1) or not (0)
- department: The department in which the employee works
- salary: The salary level of the employee (low, medium, high)

## Project Pipeline

### Exploratory Data Analysis (EDA)
An in-depth exploratory data analysis was conducted to identify the variables with the most significant impact on employee retention. Key findings include:

- Salary Impact: Bar charts were plotted to visualize the relationship between employee salaries and retention rates.
- Department Correlation: Bar charts illustrated the correlation between departments and employee retention.

### Feature Selection and Preprocessing
Based on the EDA results, the most impactful variables were selected for the model:
- Satisfaction Level, Average Monthly Hours, Promotion Last 5 Years and Salary

Preprocessing steps included:
- Label Encoding: Applied to categorical variables, particularly the 'salary' feature, to convert it into a numerical format.
- Standard Scaling: Utilized to normalize numerical features, ensuring all variables are on the same scale for optimal model performance.

### Model Development
A Random Forest Classifier model was built using the selected features:

- Data Splitting: The dataset was divided into training and testing sets.
- Model Training: A Random Forest Classifier model was trained on the training data.

### Model Evaluation
The model's performance was evaluated using the following metrics:

- Accuracy: [Insert accuracy score]
- Precision: [Insert precision score]
- Recall: [Insert recall score]
- F1-Score: [Insert F1-score]

![image](https://github.com/user-attachments/assets/77262c49-ee30-443c-ac20-b562eff0366c)


### Gradio App Development
A Gradio app was created to provide an interactive interface for predicting employee attrition:

- Input Features: The app allows users to input employee data through a user-friendly interface.
- Prediction: The trained Random Forest Classifier model is utilized to predict the likelihood of attrition.
- Visualization: Results are displayed clearly, potentially including probability scores and interpretable insights.

## Future Improvements

- Experiment with other machine learning algorithms for comparison.
- Incorporate more advanced feature engineering techniques.
- Develop a more comprehensive dashboard with additional HR insights.
- Implement continuous integration/continuous deployment (CI/CD) for the ML pipeline.
