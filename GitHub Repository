import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
import pickle

data = {
    'Hours_Studied': [1,2,3,4,5,6,7,8,2,3,5,6,7,8,9,4,5,6,7,8],
    'Sleep_Hours': [7,6,6,5,7,8,6,5,7,6,8,7,6,5,8,7,6,7,6,5],
    'Attendance': [60,65,70,75,80,85,90,95,60,70,80,85,90,95,100,75,85,80,90,95],
    'Marks': [30,35,45,50,60,70,75,85,40,50,65,72,78,88,95,55,68,75,82,90]
}

df = pd.DataFrame(data)
X = df[['Hours_Studied', 'Sleep_Hours', 'Attendance']]
y = df['Marks']

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

model = LinearRegression()
model.fit(X_train, y_train)
y_pred = model.predict(X_test)

print("MAE:", round(mean_absolute_error(y_test, y_pred), 2))
print("MSE:", round(mean_squared_error(y_test, y_pred), 2))
print("R² Score:", round(r2_score(y_test, y_pred), 2))

plt.scatter(y_test, y_pred, color='blue')
plt.plot([min(y_test), max(y_test)], [min(y_test), max(y_test)], color='red', linestyle='--')
plt.xlabel("Actual Marks")
plt.ylabel("Predicted Marks")
plt.title("Actual vs Predicted Marks")
plt.show()

with open('student_marks_model.pkl', 'wb') as file:
    pickle.dump(model, file)

hours = float(input("Enter study hours: "))
sleep = float(input("Enter sleep hours: "))
attendance = float(input("Enter attendance (%): "))

with open('student_marks_model.pkl', 'rb') as file:
    loaded_model = pickle.load(file)

predicted_marks = loaded_model.predict([[hours, sleep, attendance]])
print("Predicted Marks:", round(predicted_marks[0], 2))

plt.scatter(df['Hours_Studied'], df['Marks'], label='Dataset', color='orange')
plt.scatter(hours, predicted_marks, label='Predicted', color='green', s=100)
plt.xlabel("Hours Studied")
plt.ylabel("Marks")
plt.title("Prediction on Dataset")
plt.legend()
plt.show()
