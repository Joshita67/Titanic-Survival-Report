# Titanic-Survival-Report
This project uses machine learning to predict Titanic passenger survival based on factors like age, gender, and ticket class. It includes data preprocessing (missing values, encoding, normalization), model training, and evaluation with metrics like accuracy and precision. Results, code, and insights are documented in a GitHub repository.
Titanic Survival Prediction Project
Overview
This project leverages machine learning to predict the survival status of Titanic passengers based on various features like age, gender, ticket class, and fare. Using Python and data science libraries, the dataset undergoes preprocessing, model training, evaluation, and performance analysis.

Dataset
The dataset contains information about Titanic passengers:

PassengerId: Unique identifier for each passenger.

Survived: Survival status (0 = Did not survive, 1 = Survived).

Pclass: Ticket class (1st, 2nd, 3rd class).

Name: Passenger name.

Sex: Gender.

Age: Age of the passenger.

SibSp & Parch: Number of siblings/spouses and parents/children aboard.

Ticket: Ticket number.

Fare: Ticket fare paid.

Cabin: Cabin number.

Embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

Steps
1. Data Preprocessing
Missing Values: Handled Age, Embarked with median and mode imputation; dropped Cabin due to excessive missing data.

Categorical Encoding: Converted Sex and Embarked to numeric using LabelEncoder.

Feature Scaling: Normalized numerical variables like Age and Fare using StandardScaler.

2. Model Training
Used a Random Forest Classifier as the base model to predict passenger survival:

Train-Test Split: Split data into 80% training and 20% testing.

Hyperparameter Tuning: Experimented with model settings for optimal performance.

3. Evaluation Metrics
Assessed model performance using:

Accuracy: Percentage of correct predictions.

Precision: Proportion of true positive predictions.

Recall: Ability of the model to detect positive cases.

F1 Score: Balance between precision and recall.

Confusion Matrix: Visualized prediction results.

4. Results
The model achieved satisfactory prediction accuracy on the test dataset and demonstrated stability across cross-validation.

Repository Structure
titanic-survival-prediction/
├── data/
│   └── tested.csv (Dataset file)
├── notebooks/
│   └── titanic_prediction.ipynb (Jupyter Notebook containing code)
├── models/
│   └── titanic_model.pkl (Trained model file)
├── README.md (Project description)
