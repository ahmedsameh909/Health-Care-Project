# 🫀 Healthcare Project: Indicators of Heart Disease (2022 Update)
## live view https://health-care-project.streamlit.app/
## 📊 1. Dataset Description

This project uses the **“Indicators of Heart Disease (2022 Update)”** dataset.  
The dataset contains health-related information collected from U.S. adults to identify factors that may increase the risk of heart disease.

- **Number of Rows:** 445,132  
- **Number of Columns:** 40  
- **Source:** [Kaggle - Indicators of Heart Disease (2022)](https://www.kaggle.com)  
- **Objective:** Analyze the dataset, clean and preprocess it, then prepare it for data visualization and predictive modeling.

### 🧾 Feature Overview

| Feature                          | Description |
|-----------------------------------|-------------|
| `State`                           | U.S. state of residence |
| `Sex`                             | Biological sex of the participant |
| `GeneralHealth`                   | Self-rated general health |
| `PhysicalHealthDays`              | Number of days physical health was not good |
| `MentalHealthDays`                | Number of days mental health was not good |
| `LastCheckupTime`                 | Time since last routine checkup |
| `PhysicalActivities`              | Whether the participant engaged in physical activities |
| `SleepHours`                      | Average hours of sleep per night |
| `RemovedTeeth`                    | Number of permanent teeth removed |
| `HadHeartAttack`                  | History of heart attack (Yes/No) |
| `HadAngina`                       | History of angina or coronary heart disease |
| `HadStroke`                       | History of stroke |
| `HadAsthma`                       | History of asthma |
| `HadSkinCancer`                   | History of skin cancer |
| `HadCOPD`                         | History of chronic obstructive pulmonary disease |
| `HadDepressiveDisorder`           | History of depressive disorder |
| `HadKidneyDisease`               | History of kidney disease |
| `HadArthritis`                   | History of arthritis |
| `HadDiabetes`                    | History of diabetes |
| `DeafOrHardOfHearing`            | Hearing difficulties |
| `BlindOrVisionDifficulty`       | Vision difficulties |
| `DifficultyConcentrating`       | Difficulty concentrating or remembering |
| `DifficultyWalking`             | Difficulty walking or climbing stairs |
| `DifficultyDressingBathing`     | Difficulty dressing or bathing |
| `DifficultyErrands`            | Difficulty doing errands alone |
| `SmokerStatus`                 | Smoking status |
| `ECigaretteUsage`              | E-cigarette usage |
| `ChestScan`                    | History of chest CT scan |
| `RaceEthnicityCategory`        | Race and ethnicity |
| `AgeCategory`                  | Age group |
| `HeightInMeters`              | Height in meters |
| `WeightInKilograms`           | Weight in kilograms |
| `BMI`                          | Body Mass Index |
| `AlcoholDrinkers`             | Alcohol consumption |
| `HIVTesting`                  | HIV testing status |
| `FluVaxLast12`                | Flu vaccination in the last 12 months |
| `PneumoVaxEver`               | Pneumococcal vaccination |
| `TetanusLast10Tdap`           | Tetanus vaccination in the last 10 years |
| `HighRiskLastYear`           | High risk for severe illness in the last year |
| `CovidPos`                    | COVID-19 positivity status |

---

## 🧹 2. Step 1: Data Cleaning

Data cleaning ensures data quality, consistency, and reliability for analysis.  
The following steps were applied:

- **Handling Missing Values:**  
  - Identified missing values across all columns.  
  - Applied appropriate strategies (drop or impute) depending on data importance.

- **Text Standardization:**  
  - Unified categorical values (e.g., `Yes` / `No`) and removed extra spaces.  
  - Normalized text casing.

- **Duplicate Removal:**  
  - Checked for duplicate records and removed them to avoid redundancy.

- **Data Type Conversion:**  
  - Converted numeric columns like `HeightInMeters`, `WeightInKilograms`, `BMI`, and health day counts to numeric types.  
  - Converted categorical variables to `category` type for optimization.

- **Inconsistency Check:**  
  - Fixed inconsistent values and ensured standardized labels across categorical fields.

---

## 📈 3. Step 2: Data Visualization & Preprocessing

### 🖼️ Data Visualization

To understand the data distribution and detect hidden patterns:

- Plotted the **distribution of heart-related conditions** (`HadHeartAttack`, `HadAngina`, etc.).  
- Explored relationships between **BMI**, **AgeCategory**, and **Sex** with heart disease indicators.  
- Visualized **vaccination**, **smoking**, and **alcohol habits** impact on health indicators.  
- Detected outliers in numerical features (`BMI`, `SleepHours`, `PhysicalHealthDays`) using boxplots.  
- Checked data balance for key target variables.

### ⚙️ Data Preprocessing

Prepared the dataset for modeling:

- **Encoding:**  
  - Transformed categorical columns into numeric format using One-Hot Encoding or Label Encoding.

- **Scaling:**  
  - Standardized numerical columns to improve model performance.

- **Balancing:**  
  - Addressed class imbalance for target features like `HadHeartAttack` if necessary.

- **Splitting:**  
  - Divided data into training and testing sets for future predictive modeling.

--

## 🛠️ Tools & Libraries

- [Python](https://www.python.org/)  
- [Pandas](https://pandas.pydata.org/)  
- [NumPy](https://numpy.org/)  
- [Matplotlib](https://matplotlib.org/)  
- [Seaborn](https://seaborn.pydata.org/)  
- [Scikit-learn](https://scikit-learn.org/)

--
# 🤖 4. Machine Learning Modeling (Extended Version)

After preparing the dataset through cleaning, encoding, scaling, and balancing, we developed a complete **ML pipeline** to predict heart-related outcomes such as `HadHeartAttack`.

---

## 🔍 Modeling Objectives

- Identify the **best-performing algorithm**  
- Build a **stable and generalizable** prediction model  
- Improve **classification performance** on imbalanced classes  
- Achieve high **accuracy** and **recall** to minimize false negatives  

---

## 🔧 Algorithms Used

We experimented with several supervised classification algorithms:

| Model | Notes |
|-------|-------|
| **Logistic Regression** | Baseline model, good interpretability |
| **Random Forest Classifier** | Handles non-linearity well |
| **XGBoost Classifier** | Best performance, robust with imbalanced data |

---

## ⚙️ Modeling Pipeline

1. **Split Dataset**  
   - 80% training, 20% testing  

2. **Train Models**  
   - Fit each model on balanced training data  

3. **Hyperparameter Tuning**  
   - GridSearchCV for Random Forest & XGBoost  

4. **Evaluate Models**  
   - Accuracy, Precision, Recall, F1-score  

5. **Visualize**  
   - Confusion Matrix  
   - ROC-AUC Curve  

6. **Save Best Model**  
   - Exported using **Joblib**  

**Best Model:** **XGBoost Classifier**

---

# ☁️ 5. Streamlit Deployment (Extended Version)

After finalizing the ML model, we deployed the system using **Streamlit**, enabling **real-time heart-risk predictions** through an interactive web interface.

---

## 🖥️ Why Streamlit?

- Lightweight and easy to deploy  
- Real-time predictions  
- Simple UI for non-technical users  
- Built for ML model deployment  

---

## 🧪 Streamlit Features

### 1️⃣ Real-Time Prediction

Users enter their health indicators such as:

- **Age**  
- **BMI**  
- **Physical Activity**  
- **Smoking Status**  
- **Chronic Conditions**  

Streamlit processes the input → sends it to the **XGBoost model** → returns the risk result instantly.

---

### 2️⃣ Dynamic Visualization

- Shows charts and insights directly inside the app  
- Helps users understand the **impact of each feature**  

---

### 3️⃣ Chatbot Integration (Gemini API)

We added a built-in chatbot that helps users:

- Understand medical terms  
- Interpret prediction results  
- Ask health-related questions  

**Example Questions:**

- “What does BMI mean?”  
- “Is smoking affecting my risk?”  
- “Why is my result high?”  

The chatbot responds using the **Google Gemini API**.


## 📌 Team
**Ahmed Sameh**  
**AbdalluH Ahmed**  
**Mohamed Yasser**  
**Rewan Adel**  


