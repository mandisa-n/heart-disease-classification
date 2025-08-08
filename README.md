## Classification of Heart Disease Using Logistic Regression

## Project Overview  
This project uses **Logistic Regression** to predict the presence of heart disease based on 14 medical attributes. The dataset includes patient demographics, clinical measurements, and diagnostic test results. The goal is to classify whether a patient is likely to have heart disease.

## Objective  
To develop a classification model that predicts the presence of heart disease using health-related features.

## Dataset  
- **Rows:** 303 
- **Columns:** 14  
  - `age`: Age in years  
  - `sex`: Gender (1 = male, 0 = female)  
  - `cp`: Chest pain type (0 = typical angina, 1 = atypical angina, 2 = non-anginal pain, 3 = asymptomatic)  
  - `chol`: Serum cholesterol in mg/dl  
  - `trestbps`: Resting blood pressure (mm Hg)  
  - `fbs`: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)  
  - `thalach`: Maximum heart rate achieved  
  - `restecg`: Resting electrocardiogram results  
  - `exang`: Exercise-induced angina (1 = yes, 0 = no)  
  - `oldpeak`: ST depression induced by exercise relative to rest  
  - `ca`: Number of major vessels colored by fluoroscopy (0–3)  
  - `slope`: Slope of the peak exercise ST segment  
  - `thal`: Thalassemia  
  - `target`: Diagnosis of heart disease (1 = yes, 0 = no)  
- **Missing Values:** None  

## ⚙️ Methodology  

### 1. Data Preprocessing  
- Loaded dataset from Excel using Pandas  
- Separated features into continuous and categorical sets  
- Converted all columns to numeric types  
- Checked and confirmed no missing values  
- Scaled features using `StandardScaler` for normalization  

### 2. Exploratory Data Analysis (EDA)  
- Previewed dataset with `.head()` and `.info()`  
- Generated descriptive statistics for categorical and continuous features  
- Visualized:  
  - Correlation heatmap  
  - Histograms for `age` and `cholesterol`  
  - Bar plots for heart disease distribution by gender and ECG results  

### 3. Model Training  
- Defined features (`X`) and target (`y`)  
- Split data into training (80%) and testing (20%) sets  
- Applied Logistic Regression model from scikit-learn  
- Trained model on scaled training data  

### 4. Model Evaluation  
- Calculated accuracy score  
- Generated confusion matrix (visualized with heatmap)  
- Computed cross-entropy loss, precision, recall, F1-score  
- Plotted ROC curve and computed AUC  

## Results  
- **Accuracy:** 85%
- **Precision:** 0.871  
- **Recall:** 0.844  
- **F1-score:** 0.857  
- **ROC AUC Score:** 0.927   

## Technologies Used  
- Python  
- Libraries:  
  - NumPy, Pandas  
  - Matplotlib, Seaborn  
  - scikit-learn  
