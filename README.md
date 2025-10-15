# 🫀 Healthcare Project: Indicators of Heart Disease (2022 Update)

## 📊 1. Dataset Description

The dataset used in this project is **“Indicators of Heart Disease (2022 Update)”**.  
It contains health-related information collected to identify patterns and factors that may increase the risk of heart disease.

- **Number of Rows:** 400K+
- **Number of Columns:** 40 
- **Source:** [Kaggle - Indicators of Heart Disease](https://www.kaggle.com)  
- **Goal:** Analyze the data to identify factors correlated with heart disease and prepare it for further machine learning models.

### 🧾 Features Overview:
- `HeartDisease` → Target variable (Yes/No)  
- `BMI` → Body Mass Index  
- `Smoking` → Whether the person has smoked at least 100 cigarettes in their life  
- `AlcoholDrinking` → Heavy drinker or not  
- `Stroke` → Whether the person has ever had a stroke  
- `PhysicalHealth`, `MentalHealth` → Number of unhealthy days in the past 30 days  
- `DiffWalking` → Difficulty walking or climbing stairs  
- `Sex` → Male or Female  
- `AgeCategory` → Age group of the person  
- `Race` → Ethnicity of the person  
- `Diabetic` → Diabetic status  
- `PhysicalActivity` → Physical activity or not  
- `GenHealth` → General health status  
- `SleepTime` → Average sleep time in hours  
- `Asthma`, `KidneyDisease`, `SkinCancer` → Medical history indicators

---

## 🧹 2. Step 1: Data Cleaning

Data cleaning is an essential step to ensure the quality and consistency of the dataset.  
The following actions were performed:

- **Handling Missing Values:**  
  - Checked for null values and handled them appropriately (removal or imputation).

- **Standardizing Text Values:**  
  - Unified categorical values (e.g., `Yes` / `No`) and removed unnecessary spaces.

- **Removing Duplicates:**  
  - Identified and dropped duplicate rows to avoid bias.

- **Checking Data Types:**  
  - Converted numeric columns to their correct formats and categorical columns to categories.

- **Correcting Inconsistencies:**  
  - Fixed typos, standardized labels, and cleaned string fields.

---

## 📈 3. Step 2: Data Visualization & Preprocessing

### 🖼️ Data Visualization
Exploratory analysis was conducted to understand data distribution and patterns:

- Plotted **distribution of heart disease cases**.  
- Explored relationships between **BMI**, **SleepTime**, and **AgeCategory** with heart disease.  
- Visualized categorical variables (e.g., Smoking, Stroke) using bar plots and count plots.  
- Detected and examined outliers using boxplots.

### ⚙️ Data Preprocessing
Prepared the dataset for further analysis and modeling:

- **Encoding:** Applied One-Hot or Label Encoding to categorical variables.  
- **Scaling:** Normalized/standardized numerical columns (BMI, SleepTime, etc.).  
- **Balancing:** Addressed class imbalance if necessary.  
- **Splitting:** Divided the dataset into training and testing sets.

---



## 🛠️ Tools & Libraries
- [Python](https://www.python.org/)  
- [Pandas](https://pandas.pydata.org/)  
- [NumPy](https://numpy.org/)  
- [Matplotlib](https://matplotlib.org/)  
- [Seaborn](https://seaborn.pydata.org/)  
- [Scikit-learn](https://scikit-learn.org/)

---

## 📌 Team
**Ahmed Sameh**  
**AbdalluH Ahmed**  
**Mohamed Yasser**  
**Rewan Adel**  


