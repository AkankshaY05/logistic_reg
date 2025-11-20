# logistic_reg
This project applies Logistic Regression to predict whether a passenger survived the Titanic disaster. Logistic Regression is a supervised machine learning algorithm used for binary classification tasks.

📂 2. Dataset

Dataset used (loaded directly from URL):

https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv


Target variable:

Survived → 1 (survived), 0 (not survived)

🧹 3. Data Preprocessing

Key preprocessing steps:

Dropped irrelevant columns: Name, Ticket, Cabin

Encoded categorical features (Sex, Embarked)

Filled missing values (Age → median, Embarked → mode)

Train–test split (80–20)

Standardized features using StandardScaler

🤖 4. Model

Model used:

Logistic Regression (sklearn.linear_model.LogisticRegression)

Trained on standardized data

Predicted both labels & probabilities

📊 5. Evaluation Metrics

Metrics used to evaluate the model:

Confusion Matrix

Accuracy, Precision, Recall, F1-score

ROC Curve & AUC Score

Threshold tuning to examine probability cutoffs

🧠 6. Sigmoid Function

Logistic Regression uses the sigmoid function to convert model output into probabilities:

𝜎
(
𝑧
)
=
1
1
+
𝑒
−
𝑧
σ(z)=
1+e
−z
1
	​
