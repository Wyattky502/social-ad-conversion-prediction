# Social Ad Conversion Prediction

This project builds a logistic regression model to predict whether a user will purchase a product based on their age and estimated salary, using data from social media advertisements. 

## Project Overview
The goal of this analysis is to determine the strongest demographic predictors for ad conversion. By establishing a reliable predictive model, marketing teams can better target their advertising spend toward high-converting user segments.

## Methodology
This project utilizes a standard machine learning pipeline via `scikit-learn`:
1.  **Data Preprocessing:** Categorical target variables were converted to binary classifiers.
2.  **Feature Scaling:** Input features (Age and Estimated Salary) were standardized using `StandardScaler` to allow for direct comparison of their impact.
3.  **Model Training:** A Logistic Regression model was trained on a 75/25 train-test split.
4.  **Evaluation:** The model was evaluated using accuracy scoring and a confusion matrix. The underlying log-odds math was also manually verified against the model's predictive output.

## Key Findings
* **Model Accuracy:** The logistic regression model achieved an **89.00% accuracy** on unseen test data, indicating a robust fit.
* **Feature Importance:** Age is the primary driver of purchase behavior. For every one standard deviation increase in a user's age, the log-odds of a purchase increase by **2.08**. 
* **Secondary Driver:** Estimated Salary is also a positive predictor, though less impactful, increasing the log-odds of a purchase by **1.11** per standard deviation.

## Technologies Used
* **Python 3**
* **Pandas** (Data Manipulation)
* **Scikit-Learn** (Machine Learning & Preprocessing)
* **Matplotlib** (Data Visualization)
* **NumPy** (Mathematical Verification)

## How to Run
To run this project locally, ensure you have the required libraries installed. Clone this repository, and open the `Ad_conversion_prediction.ipynb` file in Jupyter Notebook or JupyterLab. Ensure the `social_ads.csv` file is located in the same directory as the notebook.
