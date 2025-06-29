Based on the analysis of your notebook **"Sleep Health Lifestyle"**, here's a detailed and well-structured `README.md` file:

---

# 💤 Sleep Health & Lifestyle – Sleep Disorder Prediction

This project focuses on identifying patterns and building a machine learning model to predict **sleep disorders** based on individuals' health and lifestyle factors. The model helps classify whether a person is likely to suffer from **Sleep Apnea**, **Insomnia**, or has **No Disorder** using clinical and demographic data.

---

## 📌 Project Highlights

* 🧠 Predictive modeling for **Sleep Disorders** using supervised machine learning
* 📊 Rich **EDA** to explore relationships between profession, BMI, gender, blood pressure, and sleep issues
* 🧼 Includes data cleaning, label encoding, feature engineering, and model evaluation
* 🤖 Built and evaluated models: **Logistic Regression**, **Decision Tree**, and **Random Forest**
* 💾 Final model is saved for deployment/inference use

---

## 📁 Dataset

* **Source**: [Kaggle Sleep Health and Lifestyle Dataset](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)
* **Records**: 374 individuals
* **Features**:

  * Gender, Age, Occupation
  * BMI Category
  * Blood Pressure (converted to Upper/Lower BP)
  * Heart Rate, Sleep Duration, Physical Activity Level, Stress Level
  * Target: `Sleep Disorder` (Insomnia, Sleep Apnea, No Disorder)

---

## 🧪 Workflow

### 1. Data Acquisition

* Used Kaggle API and Colab integration to download dataset.

### 2. Data Preprocessing

* Converted Blood Pressure from string to numeric format (split into `Upper BP`, `Lower BP`)
* Handled missing values in the `Sleep Disorder` column by labeling as `'No Disorder'`
* Dropped irrelevant columns like `Person ID`
* Label encoded categorical variables

### 3. Exploratory Data Analysis (EDA)

* Visualized class distribution using **Plotly** histograms
* Analyzed correlations using **pairplots**, **countplots**, and **pie charts**
* Key insights:

  * Sleep Apnea is more prevalent in females
  * Insomnia is more common among males and salespeople
  * Overweight individuals and those with high stress have higher chances of sleep disorders

### 4. Model Building

* Trained and evaluated:

  * Logistic Regression
  * Decision Tree Classifier
  * Random Forest Classifier
* Used **Train-Test Split** for evaluation

### 5. Model Saving

* Best-performing model saved using `joblib` for future inference.

---

## 📊 Tools & Technologies

* **Languages**: Python
* **Libraries**: Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Plotly
* **Platform**: Google Colab, Kaggle API

---

## 📈 Visualizations

* 📍 **Pairplots** showing clusters of sleep disorder types
![alt text](images/image.png)
* 📍 **Pie charts** and **histograms** for class-wise distributions
![alt text](images/image-1.png)
![alt text](images/image-4.png)
![alt text](images/image-3.png)
* 📍 **Countplots** for gender and occupation analysis
![alt text](images/image-2.png)
---

## 🧠 Outcome

This project demonstrates the effectiveness of machine learning in analyzing health-related data and predicting sleep disorders. The final model can be integrated into health-monitoring systems to provide early insights and suggest lifestyle changes for better sleep hygiene.


