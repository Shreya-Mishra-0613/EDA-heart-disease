# 🫀 Task 2: Exploratory Data Analysis (EDA) on Heart Disease Dataset

## 📌 Objective
The goal of this task was to perform Exploratory Data Analysis (EDA) to uncover patterns, trends, and anomalies in the dataset that may help in understanding the likelihood of heart disease based on patient health parameters.

---

## 📁 Dataset Overview
The dataset consists of multiple health-related features for individuals, such as:
- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar
- Resting ECG
- Max Heart Rate
- Exercise-induced Angina
- Oldpeak (ST depression)
- ST Slope
- Target (HeartDisease)

---

## 🔍 What I Did
- Loaded and cleaned the dataset using **Pandas**
- Performed **univariate analysis** using histograms, boxplots, and countplots to explore the distribution of each feature
- Conducted **bivariate analysis** between features and the target variable (`HeartDisease`) using:
  - Boxplots and Violinplots for numerical variables
  - Countplots with hue for categorical features
  - Pairplots to study feature relationships
- Explored **correlations** to assess multicollinearity and feature relevance

---

## 📊 Key Insights from EDA

### 🔹 Gender & Chest Pain
- Males are significantly more likely to suffer from heart disease
- People with **Asymptomatic (ASY)** chest pain are most likely to have CVD

### 🔹 Glucose, ECG & Angina
- People with **higher fasting blood sugar (FastingBS = 1)** are more prone to heart disease
- ST-T wave abnormality on resting ECG is associated with a higher chance of CVD
- Exercise-induced angina is a strong indicator of underlying heart issues

### 🔹 ST Slope & Heart Performance
- People with **Flat or Downward ST slopes** are more likely to have heart disease
- Higher **Oldpeak** (ST depression) values are positively correlated with CVD
- Lower **MaxHR** values are negatively correlated with heart health — higher max heart rate → better condition

### 🔹 Age, Blood Pressure & Cholesterol
- Heart disease is more common among **older people**
- **RestingBP** shows little correlation with heart disease
- **Cholesterol** contains many **zero values**, indicating data inconsistency or entry errors

---

## 📈 Distribution Insights

- **Age**: Normally distributed, no outliers
- **RestingBP**: Negatively skewed with outliers at both low (0) and high (~200) ends
- **Cholesterol**: Positively skewed; 0 values are biologically invalid
- **MaxHR**: Near-normal distribution with a few outliers
- **Oldpeak**: Highly skewed with noticeable outliers; useful for diagnosis

---

## 📉 Population Characteristics

- Around **79% of patients are male**
- Majority experience **Asymptomatic chest pain**
- Most have **normal fasting blood sugar and ECG**
- About **60%** did **not experience exercise-induced angina**
- Most have **Up or Flat ST Slope**
- Over **55% of individuals have heart disease**

---

## 🧠 Learnings

- Understood how to perform and interpret **univariate and bivariate analysis**
- Learned how different types of visualizations (boxplot, violinplot, countplot) help reveal insights
- Gained awareness of data issues such as **skewness, outliers, and entry errors**
- Developed ability to relate medical features with disease outcomes using data analysis

---

## 🔧 Tools Used
- Python
- Pandas
- Seaborn
- Matplotlib
- Jupyter Notebook

---

## ✅ Conclusion
This EDA task helped me understand the underlying structure of health data and how visualizations and statistics can be used to uncover patterns related to heart disease. It also highlighted the importance of clean and accurate data for reliable analysis.

