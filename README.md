🫀 Healthcare Project: Indicators of Heart Disease (2022 Update)
📊 1. Dataset Description

The dataset used in this project is “Indicators of Heart Disease (2022 Update)”.
It contains health-related information collected to identify patterns and factors that may increase the risk of heart disease.

Number of Rows: 319,795

Number of Columns: 18

Source: Kaggle - Indicators of Heart Disease

Goal: Analyze the data to identify factors correlated with heart disease and prepare it for further machine learning models.

🧾 Features Overview:

HeartDisease → Target variable (Yes/No)

BMI → Body Mass Index

Smoking → Whether the person has smoked at least 100 cigarettes in their life

AlcoholDrinking → Heavy drinker or not

Stroke → Whether the person has ever had a stroke

PhysicalHealth, MentalHealth → Number of unhealthy days in the past 30 days

DiffWalking → Difficulty walking or climbing stairs

Sex → Male or Female

AgeCategory → Age group of the person

Race → Ethnicity of the person

Diabetic → Diabetic status

PhysicalActivity → Physical activity or not

GenHealth → General health status
🧹 2. Step 1: Data Cleaning

Data cleaning is an essential step to ensure the quality and consistency of the dataset.
In this step, the following actions were taken:

Handled missing values:

Checked for null values and handled them appropriately (removal or imputation).

Standardized text values:

Cleaned and unified categorical values (e.g., Yes / No).

Removed duplicates:

Checked for duplicate rows and dropped them to avoid bias.

Checked data types:

Converted numeric columns to the correct format and categorical columns to categories.

Corrected inconsistent entries:

Removed spaces, fixed typos, and standardized labels.

📈 3. Step 2: Data Visualization & Preprocessing
🖼️ Data Visualization:

To better understand the dataset and detect patterns:

Plotted distribution of heart disease cases.

Explored BMI, SleepTime, and AgeCategory relationships with heart disease.

Visualized categorical features (Smoking, Stroke, etc.) using bar plots and count plots.

Checked for outliers using boxplots.

⚙️ Data Preprocessing:

To prepare the dataset for modeling:

Encoded categorical variables using One-Hot Encoding / Label Encoding.

Normalized or standardized numerical columns (BMI, SleepTime, etc.).

Balanced the dataset if needed (e.g., handling class imbalance).

Split the data into training and testing sets.

SleepTime → Average sleep time in hours

Asthma, KidneyDisease, SkinCancer → Medical history indicators
