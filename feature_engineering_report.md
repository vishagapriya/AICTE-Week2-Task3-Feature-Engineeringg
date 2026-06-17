# Feature Engineering Report

## Dataset

The Titanic dataset was used for this task. The dataset contains passenger information such as age, gender, passenger class, fare, and survival status.

## Data Preprocessing

Missing values were handled using suitable imputation techniques. Numerical columns were filled using mean values and categorical columns were filled using the most frequent values.

## Feature Engineering

Two new features were created:

* FamilySize = SibSp + Parch + 1
* IsAlone = 1 if the passenger was travelling alone, otherwise 0

These features were created to better represent family relationships among passengers.

## Encoding

Categorical variables were converted into numerical values using Label Encoding so that they could be used by machine learning algorithms.

## Feature Scaling

StandardScaler was applied to normalize the feature values and improve consistency across different variables.

## Feature Selection

SelectKBest with the Chi-Square test was used to identify the most relevant features for predicting passenger survival.

## Outcome

The selected features were saved in the file `selected_features.csv`. Feature engineering and selection helped reduce unnecessary information and improve the quality of the dataset for machine learning tasks.
