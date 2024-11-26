# Heart-Attack-Analysis-Prediction

This project focuses on building a **Machine Learning (ML) model** to predict how prone a person is to a heart attack based on various health and lifestyle indicators.  
The project was developed as part of the course **Introduction to Machine Learning (CSL2010)**.

---

## 📊 Dataset Overview

The dataset contains **303 samples** and **14 columns**, including patient details and medical observations.  

### Features:

- **`Age`**: Patient's age in years.  
- **`Sex`**: Patient's gender.  
- **`cp`**: Type of chest pain experienced:  
  - `1`: Typical angina  
  - `2`: Atypical angina  
  - `3`: Non-anginal pain  
  - `4`: Asymptomatic  
- **`trtbps`**: Resting blood pressure (mm Hg).  
- **`chol`**: Cholesterol level (mg/dl).  
- **`fbs`**: Fasting blood sugar > 120 mg/dl (`1` = true, `0` = false).  
- **`rest_ecg`**: Resting electrocardiogram results:  
  - `0`: Normal  
  - `1`: ST-T wave abnormality  
  - `2`: Left ventricular hypertrophy (Estes' criteria).  
- **`thalach`**: Maximum heart rate achieved during physical exertion.  
- **`exng`**: Exercise-induced angina (`1` = yes, `0` = no).  
- **`oldpeak`**: Previous peak (ST depression induced by exercise).  
- **`slp`**: Slope of the peak exercise ST segment.  
- **`caa`**: Number of major vessels visible through fluoroscopy (range: `0-3`).  
- **`thall`**: Thal Rate.  

### Output Variable:
- **`target`**: Predicted likelihood of a heart attack (`0` = lower risk, `1` = higher risk).  

### Column Categorization:
- **`categorical_cols`** = ["sex", "cp", "fbs", "exng", "restecg", "thall", "caa", "slp"]
- **`continuous_cols`** = ["age", "trtbps", "chol", "thalachh", "oldpeak"]

## 🛠️ Data Preprocessing and Analysis Workflow

### Exploratory Data Analysis (EDA):

Visualizations like histograms, box plots, and scatter plots are created to identify feature distributions, relationships, and potential outliers.

### Train-Test Split:

The dataset is split into training and testing sets to evaluate model performance while avoiding `data leakage`.

### Scaling Continuous Features:

Continuous features are standardized using `StandardScaler` to ensure they have a mean of `0` and a standard deviation of `1`.

## 🚀 Models Implemented

The following ML models were implemented and evaluated for this project:
- Logistic Regression
- Gaussian Naive Bayes
- Bernoulli Naive Bayes
- Support Vector Machine (SVM)
- Decision Tree Classifier
- K-Nearest Neighbors (KNN)
- Multi-Layer Perceptron (MLP)

## 📈 Results

### Model Performance:

Each model was evaluated using metrics such as accuracy, precision, recall, and F1-score.
Comparative analysis of these metrics helped identify the most effective model for predicting heart attack risks.

## 🧑‍💻 Team Members

- Ayaan Choudhury (B23ME1013)
- Arush Aaron John (B23CH1009)
- Harsh Nandan Shukla (B23MT1019)
- Saketh Babburu (B23ME1059)

## 🤝 Acknowledgments

This project was completed under the guidance of Prof. Avinash Sharma for the course `Introduction to Machine Learning (CSL2010)`.
