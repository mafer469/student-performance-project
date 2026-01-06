# Student Performance Predictor

> **AI-powered student performance predictor system trained on a Student Performance dataset.**  
Helping students predict their performance based on their lifestyle and study habits.

---

## Overview
**Student Performance Predictor** is a project that predicts a student's performance score based on study habits, previous scores, sleep hours, practice, and extracurricular activities. It is designed to demonstrate an end-to-end machine learning workflow, including:
- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering
- Model training and evaluation
- User-input predictions

---

## Features
- **EDA:** Explore relationships between study habits, extracurricular activities, and performance.
- **Models:** Linear Regression (primary) and Random Forest (comparison).
- **Metrics:** RMSE, MAE, R^2 for model evaluation
- **User Input Demo:** Predict a student's performance interactively with a Python function.

---

## Dataset
**Source:** Kaggle [Student Performance](https://www.kaggle.com/datasets/neurocipher/student-performance?resource=download) Dataset
**Size:** 10,000 entries, 6 columns
**Features:**
- `hours_studied` - Hours spent studying
- `previous_scores` - Average previous exam scores
- `sleep_hours`- Average hours of sleep
- `sample_question_papers_practiced` - Number of practice exams completed
- `extracurricular activities_yes` - 1 if student participates in extracurricular activities, 0 otherwise
**Target:**
- performance_index: Predicted performance score
**Format:** CSV  


## Model Information
**Linear Regression:** Main predictive model, interpretable, high accuracy (R^2 ~ 0.989)
**Random Forest:** Comparison model for evaluation
**Example Metrics** (results may vary slightly due to random initialization):
| Model             | RMSE | MAE  | R² Score |
| ----------------- | ---- | ---- | -------- |
| Linear Regression | 2.02 | 1.61 | 0.989    |
| Random Forest     | 2.27 | 1.81 | 0.986    |


## User-Input Demo
To predict a  student's performance, use the `predict_student_score` function: `predict_student_score(6, 70, 7, 5, 'Yes')`
- Input the study hours, previous scores, sleep, practice, and extracurricular participation.
- The function returns the predicted `performance_index` as a float.


## Repo Structure
```
Student Performance Predictor
|
|-- data/
|   |-- student_performance.csv 
|       -> raw dataset
|
|-- notebook/
|   |-- student_performance_analysis.ipynb
|       -> Main notebook with EDA, preprocessing, modeling, and user-input demo
|
|-- README.md
```

## Setup & How to run the program

### 1. Clone the repository
```
git clone https://github.com/your-username/student-performance-project.git
```
### 2. Open the notebook in Google Colab or Jupyter Notebook
```
notebooks/Student_Performance_Predictor.ipynb
```
### 3. If using Colab, upload the CSV when prompted
### 4. Run all cells from top to bottom
### 5. Test predictions using:
```
predict_student_score(6, 70, 7, 5, 'Yes')
```

## Next Steps
- Deploy a **web app** for interactive user predictions
- Add **additional features or datasets** to enhance the model
- Explore **other ML models** for improved accuracy
