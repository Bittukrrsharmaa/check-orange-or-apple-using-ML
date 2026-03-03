# check-orange-or-apple-using-ML
🍎🍊 Fruit Classification using Decision Tree (Apple vs Orange)
📌 Project Overview

This is a simple Machine Learning classification project using Decision Tree Algorithm from Scikit-learn.

The model is trained to classify a fruit as either:

🍎 Apple

🍊 Orange

based on given features like weight and texture.

This is a beginner-friendly ML project to understand how classification works.

🛠️ Technologies Used

Python 🐍

Scikit-learn

DecisionTreeClassifier

📂 Dataset Used

The dataset is manually created inside the code:

Weight	Texture	Label
150	1	Apple
170	0	Apple
130	1	Orange
120	1	Orange
Feature Meaning:

Weight → Weight of fruit (grams)

Texture → 0 = Smooth, 1 = Rough

Label → Fruit Type (Apple/Orange)

💻 Code Implementation
# !pip install Scikit-learn

from sklearn.tree import DecisionTreeClassifier

feature = [
    [150,1],
    [170,0],
    [130,1],
    [120,1]
]

labels = ["apple","apple","orange","orange"]

clf = DecisionTreeClassifier()
clf = clf.fit(feature, labels)

prediction = clf.predict([[20,4]])

print(prediction)
📊 Output
array(['orange'], dtype='<U6')

The model predicts the fruit as Orange.

🎯 What I Learned

Basics of Machine Learning Classification

How Decision Tree works

How to train and predict using Scikit-learn

Understanding features and labels

🚀 How to Run This Project

Install Python (3.x)

Install Scikit-learn:

pip install scikit-learn

Run the Python script

📈 Future Improvements

Use real dataset instead of manual data

Add visualization of decision tree

Improve feature selection

Increase dataset size for better accuracy

👨‍💻 Author

Bittu Kumar Sharma
Aspiring Data Analyst | Machine Learning Beginner
