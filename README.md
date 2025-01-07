# Data-Science-AI-ML
# Car Price Prediction using Machine Learning

This README provides an overview of a car price prediction project using Python and machine learning.

**1. Introduction**

This project aims to build a machine learning model to predict car prices based on features such as make, engine size, curb weight, and horsepower. A CSV dataset containing car information is used.

**2. Libraries**

*   **pandas:** Data manipulation, analysis, and one-hot encoding.
*   **numpy:** Numerical computing.
*   **matplotlib.pyplot:** Basic plotting and visualization.
*   **seaborn:** Advanced statistical graphics and data visualization.
*   **sklearn.model_selection:** Data splitting (train-test) and model evaluation.
*   **sklearn.linear_model:** Linear Regression model.
*   **sklearn.metrics:** r2_score (R-squared) calculation.

**3. Data**

*   **Dataset:** A CSV file containing information about used cars.
[[CarPrice_Assignment.csv](https://github.com/user-attachments/files/18334230/CarPrice_Assignment.csv)
]
*   **Features:** Features with high correlation to price, including 'enginesize', 'curbweight', 'horsepower', 'carwidth', 'cylindernumber', 'carlength', and 'wheelbase'.
*   **Target Variable:** "Price" (the price of the car).

**4. Methodology**

1.  **Data Loading and Initial EDA:**
    *   Load the dataset using pandas.
    *   Perform initial exploratory data analysis (EDA) and visualize the data using pandas, matplotlib.pyplot, and seaborn.

2.  **Data Preprocessing:**
    *   Convert categorical variables to numerical representations using pandas one-hot encoding.
    *   Perform further EDA and visualize the processed data.

3.  **Feature Engineering:**
    *   Extract the company name from the 'CarName' feature using a lambda function and add it as a new feature.
    *   Remove redundant features ('CarName', 'car_ID', 'symboling').

4.  **Data Splitting:**
    *   Split the data into training (80%) and testing (20%) sets using `sklearn.model_selection.train_test_split`.

5.  **Model Selection and Training:**
    *   Train a Linear Regression model using `sklearn.linear_model.LinearRegression`.

6.  **Model Evaluation:**
    *   Evaluate the model's performance using the R-squared (r2_score) metric.

**5. Results and Discussion**

*   An R-squared score of 0.7952 (79%) was obtained. This means the model explains approximately 79% of the variance in car prices.

**6. Conclusion**

The analysis suggests that engine size, curb weight, horsepower, car width, cylinder number, car length, and wheelbase are significant determinants of car price.

**7. Code**

*   The code for this project is located in the repo.

**8. Dependencies**

* [List the required libraries and their versions, e.g., pandas==1.5.3, numpy==1.24.3, scikit-learn==1.2.2]

