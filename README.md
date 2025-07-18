# Employee Salary Prediction
This project aims to predict whether an employee earns more than $50K or less than or equal to $50K based on various demographic and work-related features. The project involves data loading, preprocessing, model training, evaluation, and the deployment of a web application using Streamlit.

## Dataset
The dataset used in this project is the Adult Income Dataset, which contains information about individuals from the 1994 Census database. It includes features such as age, workclass, education, marital status, occupation, relationship, race, gender, capital gain, capital loss, hours per week, native country, and income.

## Data Preprocessing
The following data preprocessing steps were performed to prepare the dataset for model training:

Handling Missing Values: Missing values represented by '?' in the 'workclass' and 'occupation' columns were replaced with 'Others'.

Removing Outliers: Outliers in the 'age' and 'educational-num' columns were removed based on box plots. The age was filtered to be between 17 and 75, and educational-num between 5 and 16.

Removing Redundant Features: The 'education' column was dropped as 'educational-num' provides similar numerical information.

Label Encoding: Categorical features such as 'workclass', 'marital-status', 'occupation', 'relationship', 'race', 'gender', and 'native-country' were converted into numerical representations using Label Encoding.

## Model Training and Evaluation
Several classification models were trained and evaluated to predict the income class:

Logistic Regression

Random Forest Classifier

K-Nearest Neighbors

Support Vector Machine

Gradient Boosting Classifier

The models were trained on the preprocessed data, and their performance was evaluated using accuracy and classification reports.

The Gradient Boosting Classifier achieved the highest accuracy of approximately 85.71%, making it the chosen model for the application.

## Streamlit Application
A web application was developed using Streamlit to provide an interactive interface for predicting employee salaries. The application allows users to input employee details through a sidebar and get a prediction of their salary class. It also supports batch prediction by uploading a CSV file.

How to Run the Streamlit App

Clone the repository:

Bash
git clone https://github.com/jaykiran-kotthakota/Employee-salary-prediction


cd Employee Salary Prediction

Install dependencies:

Bash
pip install -r requirements.txt
(Ensure you have a requirements.txt file in your repository that lists all required Python libraries, such as pandas, scikit-learn, streamlit, etc.)

Run the Streamlit application:

Bash
streamlit run app.py
(This command assumes your main Streamlit application file is named app.py. If it has a different name, please adjust accordingly.)

## About Me

LinkedIn: https://www.linkedin.com/in/jaykiran-kotthakota-787525154/


Gmail: kotthakotajaykiran@gmail.com
