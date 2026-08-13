# Fraud Detection Prediction App

A machine learning project that predicts whether a financial transaction is likely to be fraudulent based on transaction details and account balance information.

The project covers the process from data analysis and model building to deploying the trained model as a simple Streamlit web application.

## About the Project

Fraud detection is a classification problem where the goal is to identify unusual transactions while dealing with a highly imbalanced dataset.

For this project, I worked with transaction data containing information such as transaction type, transaction amount, and the sender's and receiver's account balances. I explored the data, prepared the features, trained a machine learning model, and then used the trained pipeline in a Streamlit application for prediction.

## What the Project Does

The project has two main parts:

1. **Model development** – data analysis, preprocessing, feature preparation and model training are done in `analysis_model.ipynb`.
2. **Prediction application** – the trained model is loaded into a Streamlit app where a user can enter transaction details and get a prediction.

## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Joblib
* Streamlit
* Jupyter Notebook

## Features Used

The Streamlit application takes the following inputs:

* Transaction type
* Transaction amount
* Old balance of the sender
* New balance of the sender
* Old balance of the receiver
* New balance of the receiver

The entered values are passed to the trained machine learning pipeline, which returns the prediction.

## Project Structure

```text
FraudDetectionFinal/
│
├── analysis_model.ipynb
├── fraud_detection.py
├── fraud_detection_pipeline.pkl
├── requirements.txt
├── .gitignore
└── README.md
```

### Files

**`analysis_model.ipynb`**
Contains the data analysis and machine learning workflow.

**`fraud_detection.py`**
Contains the Streamlit application used to make predictions.

**`fraud_detection_pipeline.pkl`**
Saved machine learning pipeline used by the Streamlit application.

**`requirements.txt`**
Contains the Python libraries required to run the project.

**`AIML Dataset.csv`**
The original dataset is not included in this GitHub repository because the file is too large for GitHub's regular file upload limit. It is kept locally for the project.

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/koelsaha5/Projects.git
```

### 2. Open the project folder

```bash
cd Projects
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit application

```bash
streamlit run fraud_detection.py
```

The application will open in your browser.

## Using the Application

Once the Streamlit app is running:

1. Select the transaction type.
2. Enter the transaction amount.
3. Enter the sender's old and new balance.
4. Enter the receiver's old and new balance.
5. Click **Predict**.
6. The application displays the model's prediction.

The app gives a message indicating whether the transaction is predicted to be fraudulent or not.

## Machine Learning Workflow

The project follows a basic end-to-end machine learning workflow:

```text
Dataset
   ↓
Data Exploration
   ↓
Data Preprocessing
   ↓
Feature Preparation
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Save Model Pipeline
   ↓
Streamlit Application
   ↓
Real-time Prediction
```

## What I Learned

Working on this project helped me understand how a machine learning model can be taken beyond a notebook and turned into a usable application.

Some of the main things I worked with were:

* Exploratory data analysis
* Data preprocessing
* Feature preparation
* Classification
* Handling an imbalanced fraud detection problem
* Scikit-learn pipelines
* Saving and loading trained models with Joblib
* Building a simple ML application using Streamlit

## Future Improvements

Some things I would like to improve in the future are:

* Try additional machine learning algorithms and compare their performance.
* Tune the model's hyperparameters.
* Improve the user interface of the Streamlit application.
* Add more visualizations and model performance metrics.
* Deploy the application online so that it can be accessed without running it locally.

## Author

**Koel Saha**

B.Tech Student | Aspiring Data Science & Machine Learning Professional






