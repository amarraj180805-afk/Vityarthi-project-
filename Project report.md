Student Performance Prediction Using Machine Learning

1. Introduction

Machine Learning (ML) is a branch of Artificial Intelligence that enables systems to learn patterns from data and make predictions. Predicting student performance is a critical application of ML in the education sector.
This project focuses on predicting student marks based on measurable factors such as study hours, sleep, and attendance. The goal is to help students and educators understand the impact of these factors and provide actionable insights to improve academic performance.

2. Problem Statement

Many students struggle to evaluate how their daily habits affect their academic performance. Currently, there is no simple tool to predict marks based on study routines, sleep patterns, and attendance.
Objective: Build a machine learning model capable of predicting student marks using key features such as study hours, sleep hours, and attendance percentage.

3. Objectives

Build a predictive ML model to estimate student marks.
Analyze correlations between study habits and performance.
Provide guidance to students for improving academic results.
Demonstrate real-world application of Linear Regression in AI/ML.

4. Scope of the Project

Useful for schools, colleges, and online education platforms.
Provides actionable insights for educators and parents.
Can be extended to include additional features like stress levels, extracurricular activities, and assignment scores.

5. Methodology

Data Collection: A sample dataset was created containing features: Hours Studied, Sleep Hours, Attendance, and Marks.
Data Preprocessing: Dataset was checked for consistency, and numerical values were formatted for ML.
Feature Selection: Input features: Hours_Studied, Sleep_Hours, Attendance. Target variable: Marks.
Model Selection: Linear Regression was chosen as Marks is a continuous variable.
Training and Testing: Dataset split into training (80%) and testing (20%) sets.
Model Evaluation: Metrics included MAE, MSE, RMSE, and R² Score.
Visualization: Pairplots, correlation heatmaps, and Actual vs Predicted plots were created.
Prediction Interface: Users provide study hours, sleep hours, and attendance to predict marks.

6. Tools and Technologies

Programming Language: Python
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
Platform: Terminal / Command Line
Version Control: GitHub

7. Project Implementation

Python script main.py implements all workflow steps.
Trained model is saved using pickle for future predictions.
Visualization tools help in understanding correlations and model accuracy.
Provides an interactive interface for user input to predict student marks.

8. Results

The model accurately predicts student marks for test inputs.
Observations:
Hours studied and attendance positively correlate with marks.
Sleep hours moderately affect performance.
R² score indicates strong predictive capability of the model.

9. Challenges Faced

Limited dataset size impacted prediction robustness.
Selecting the most relevant features for better accuracy.
Making the model user-friendly for non-technical users.

10. Learning Outcomes

Practical implementation of Linear Regression.
Handling and analyzing datasets using Pandas.
Data visualization with Matplotlib and Seaborn.
Understanding model evaluation metrics in ML.
Hands-on experience with saving and loading ML models.

11. Future Enhancements

Use larger, real-world datasets for improved accuracy.
Compare multiple ML algorithms (Decision Trees, Random Forests, Neural Networks).
Develop web-based or mobile interfaces for easy predictions.
Include more features such as past marks, assignments, study environment, and stress levels.
Deploy as a predictive analytics tool for educational institutions.

12. Conclusion

This project demonstrates the practical application of Machine Learning to predict student performance. The Linear Regression model provides insight into how study habits and attendance influence marks. This tool can help students improve their academic performance and assist educators in monitoring student progress.
