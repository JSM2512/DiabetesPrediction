# DiabetesPrediction

DiabetesPrediction is a machine learning project aimed at predicting the occurrence of diabetes in patients based on various medical factors. The project uses a variety of models and techniques to provide accurate predictions.

## Table of Contents

- [Overview](#overview)
- [Methodology Chart](#methodology-chart)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [Models](#models)
- [Results](#results)

## Overview

This project is designed to predict diabetes using machine learning algorithms. It utilizes the Pima Indians Diabetes Database, which includes several medical predictor variables and one target variable, Outcome. The goal is to build a model that accurately predicts whether a patient has diabetes.

### Methodology Chart
![Screenshot (420)](https://user-images.githubusercontent.com/49087609/133254918-0c71509c-e36d-40e2-994a-076edc6ba769.png)

The methodology chart outlines the DiabetesPrediction project's steps: data collection from the Pima Indians Diabetes Database, preprocessing for data quality, model training with Logistic Regression, Decision Tree, and SVM, evaluation using metrics like accuracy, integration into a Django app for real-time prediction, testing, deployment, and ongoing maintenance for accuracy and usability improvements.

## Project Structure
```
DiabetesPrediction/
├── manage.py
├── requirements.txt
├── diabetes_prediction/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── prediction/
│   ├── migrations/
│   │   └── ...
│   ├── templates/
│   │   └── ...
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
└── static/
    └── ...
```
- manage.py: Django's command-line utility for administrative tasks.
- requirements.txt: File listing the Python dependencies for the project.
- diabetes_prediction/: Django project directory containing settings and configuration.
  - settings.py: Django settings and configuration file.
  - urls.py: URL routing configuration.
  - wsgi.py: WSGI application entry point.
- prediction/: Django app directory for the prediction functionality.
  - migrations/: Directory for database migrations.
  - templates/: Directory for HTML templates.
  - admin.py: Django admin configuration.
  - apps.py: Django app configuration.
  - models.py: Django models for the app.
  - tests.py: Unit tests for the app.
  - views.py: Views handling web requests and responses.
- static/: Directory for static files (e.g., CSS, JavaScript).

## Dataset

The dataset used in this project is the Pima Indians Diabetes Database, which can be found on [Kaggle](https://www.kaggle.com/uciml/pima-indians-diabetes-database). It contains the following attributes:

1. Pregnancies
2. Glucose
3. Blood Pressure
4. Skin Thickness
5. Insulin
6. BMI
7. Diabetes Pedigree Function
8. Age
9. Outcome (target variable)

## Technologies

- Python
- Django
- MongoDB
- Jupyter Notebook
- SKLearn
- HTML
- CSS

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/JSM2512/DiabetesPrediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd DiabetesPrediction
   ```
3. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```
4. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Apply the database migrations.
   ```bash
   python manage.py migrate
   ```
2. Create a superuser to access the Django admin.
   ```bash
   python manage.py createsuperuser
   ```
3. Run the Django development server.
   ```bash
   python manage.py runserver
   ```
4. Open your web browser and go to http://127.0.0.1:8000/ to access the web interface for diabetes prediction.
5. Access the Django admin interface at http://127.0.0.1:8000/admin/ to manage the application data.

## Models

The following models have been implemented in this project:
- Random Forest
- K-Nearest Neighbors (KNN)

## Results

The performance of each model is evaluated using various metrics such as accuracy, precision, recall, and F1-score. The results are compared to determine the best-performing model.

