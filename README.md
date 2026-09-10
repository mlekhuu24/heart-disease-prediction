# heart-disease-prediction
Heart Disease Prediction is a machine learning project that predicts whether a person may have heart disease using different health and clinical features.
# Heart Disease Prediction

## Project Overview

Heart Disease Prediction is a machine learning project that predicts whether a person is likely to have heart disease based on various health and clinical features.

The project uses **Python, Pandas, Matplotlib, and Scikit-learn** to preprocess the dataset, train a Logistic Regression classification model, evaluate its performance, and make predictions for new patient data.

## Objectives

* Analyze the heart disease dataset.
* Perform data cleaning and preprocessing.
* Handle missing numerical values.
* Identify relevant health-related features.
* Train a machine learning classification model.
* Evaluate the model using accuracy, classification report, and confusion matrix.
* Predict heart disease for new input data.
* Visualize the relationship between age and cholesterol.

## Technologies Used

* **Python**
* **Pandas** – Data loading and manipulation
* **Matplotlib** – Data visualization
* **Scikit-learn** – Machine learning and evaluation

## Dataset Features

The dataset contains the following features:

| Feature               | Description                         |
| --------------------- | ----------------------------------- |
| `age`                 | Age of the person                   |
| `sex`                 | Gender indicator                    |
| `resting_bp`          | Resting blood pressure              |
| `cholesterol`         | Cholesterol level                   |
| `fasting_blood_sugar` | Fasting blood sugar indicator       |
| `max_heart_rate`      | Maximum heart rate                  |
| `chest_pain_type`     | Type of chest pain                  |
| `oldpeak`             | ST depression value                 |
| `resting_ecg`         | Resting electrocardiographic result |
| `exercise_angina`     | Exercise-induced angina indicator   |
| `st_slope`            | Slope of the ST segment             |
| `heart_disease`       | Target variable                     |

### Target Variable

* `0` – No Heart Disease
* `1` – Heart Disease

## Data Preprocessing

The project performs the following preprocessing steps:

1. Loads the dataset using Pandas.
2. Checks the dataset structure and missing values.
3. Replaces missing numerical values with their median.
4. Separates the input features and target variable.
5. Splits the dataset into training and testing sets.
6. Applies `StandardScaler` to standardize the numerical features.

## Machine Learning Algorithm

### Logistic Regression

**Logistic Regression** is used as the classification algorithm because the project has a binary target:

* 0 → No Heart Disease
* 1 → Heart Disease

The model is trained using the training dataset and then used to predict results on the testing dataset.

## Model Evaluation

The model is evaluated using:

* **Accuracy Score** – Measures the percentage of correct predictions.
* **Classification Report** – Provides precision, recall, and F1-score.
* **Confusion Matrix** – Shows correct and incorrect classification results.

## Prediction

The project also contains an example patient record with health-related values. The trained model predicts whether the example person is classified as having heart disease or not.

## Data Visualization

A scatter plot is generated to analyze the relationship between:

* **Age**
* **Cholesterol**

The visualization is saved as:

`heart_disease_analysis.png`

## Project Structure

```text
Heart_Disease_Prediction/
│
├── README.md
├── heart_disease_prediction.py
├── heart_disease.csv
├── requirements.txt
└── heart_disease_analysis.png
```

## Installation

Make sure Python is installed on your system.

Install the required libraries using:

```bash
pip install -r requirements.txt
```

## How to Run

1. Download or clone the project.
2. Open the project folder in a terminal or command prompt.
3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

4. Run the Python program:

```bash
python heart_disease_prediction.py
```

5. The program will display:

   * Dataset information
   * Missing value information
   * Model accuracy
   * Classification report
   * Confusion matrix
   * Example prediction
   * Feature visualization

## Expected Output

The program produces a model accuracy percentage along with a classification report and confusion matrix.

It also provides an example prediction such as:

```text
Example prediction: Heart Disease
```

or

```text
Example prediction: No Heart Disease
```

## Future Improvements

* Compare Logistic Regression with Random Forest, Decision Tree, SVM, and other algorithms.
* Perform hyperparameter tuning.
* Add a graphical user interface.
* Build a web application using Flask or Streamlit.
* Add more comprehensive data visualizations.
* Use a larger and clinically validated dataset.
* Deploy the model as an online prediction application.

## Disclaimer

This project is created for **educational and machine learning purposes**. It is not a medical diagnostic system and should not be used for clinical decisions. Actual medical diagnosis should always be performed by qualified healthcare professionals.
