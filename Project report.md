Conclusion
This project demonstrates the practical use of Machine Learning to predict student performance. The Linear Regression model provides insights into how study habits and attendance impact marks. This system can guide students to improve their academic performance and assist educators in monitoring student progress.
Machine Learning (ML) is a branch of Artificial Intelligence that enables systems to learn patterns from data and make predictions. Academic performance prediction is a key application of ML in the education sector.
This project predicts student marks based on measurable factors such as study hours, sleep, and attendance. The objective is to help students and educators understand which factors influence academic performance and to provide actionable insights for improvement.
2. Problem Statement
Many students are unable to evaluate how their daily habits affect their academic performance. Currently, there is no simple tool to predict marks based on their study routines and habits.
Problem: To create a machine learning model capable of predicting student marks using key features such as study hours, sleep hours, and attendance percentage.
3. Objectives
To build a predictive ML model to estimate student marks
To analyze the correlation between study habits and performance
To assist students in identifying areas to improve academic results
To demonstrate real-world application of Linear Regression in AI/ML
4. Scope of the Project
Schools, colleges, and online education platforms can use this model to predict student performance.
Provides insight into student behavior for educators and parents.
The model can be extended to include additional features like stress level, extracurricular activities, and assignment scores.
5. Methodology
Data Collection:
A sample dataset was created containing features: Hours Studied, Sleep Hours, Attendance, and Marks.
Data was organized into a structured table using Pandas DataFrame.
Data Preprocessing:
Checked dataset for consistency.
Converted all numerical values into appropriate formats for ML.
Feature Selection:
Input features: Hours_Studied, Sleep_Hours, Attendance
Target variable: Marks
Model Selection:
Linear Regression algorithm was used.
Suitable because Marks is a continuous numerical variable.
Training and Testing:
Dataset split into training (80%) and testing (20%) sets.
Model trained on training set and evaluated on testing set.
Model Evaluation:
Metrics used:
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R² Score
Visualization:
Pairplot of input features vs Marks
Correlation heatmap
Actual vs Predicted scatter plot
Prediction overlay on dataset
Prediction Interface:
Users input study hours, sleep hours, and attendance.
The model predicts the expected marks.
6. Tools and Technologies Used
Programming Language: Python
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
Platform: Terminal / Command Line
Version Control: GitHub
7. Project Implementation
Created a Python script main.py implementing all steps.
The trained model is saved using pickle for future use.
Provides user-friendly prompts for predictions.
Visualization helps in understanding correlations and prediction accuracy.
8. Results
The model predicts marks accurately for most test inputs.
Observations:
Hours studied and attendance show a strong positive correlation with marks.
Sleep hours moderately affect performance.
R² score indicates the model explains a large portion of variance in student marks.
9. Challenges Faced
Limited dataset size made prediction less robust.
Selecting the right features for improved accuracy.
Ensuring the model is understandable and user-friendly for non-technical users.
10. Learning Outcomes
Practical implementation of Linear Regression.
Handling and analyzing datasets using Pandas.

