# Housing-Price-Prediction-using-Linear-Regression
This project uses a linear regression model to predict the price of houses based on their features. The entire workflow, from data preparation to model evaluation and interpretation, is documented in the accompanying Jupyter Notebook.

---

## The Dataset

The project utilizes the `Housing.csv` dataset, which contains various attributes of houses as well as their sale prices.

---

## Project Workflow

The analysis is broken down into the following key steps:

### 1. Data Preprocessing

Before building the model, the raw data was prepared to make it suitable for analysis. This involved:
- **Converting Categorical Data**: Text-based columns with 'yes'/'no' values (like `mainroad` and `guestroom`) were converted into a numerical format (1/0).
- **One-Hot Encoding**: The `furnishingstatus` column, which has multiple categories, was converted into numerical columns.
- **Feature Scaling**: All numerical features, including the price and area, were standardized. This ensures that each feature contributes fairly to the model's predictions, regardless of its original scale.

### 2. Model Development: Linear Regression

A multiple linear regression model was built to understand the relationship between a house's features and its price.
- **Train-Test Split**: The dataset was divided into a training set (80%) and a testing set (20%). The model learns from the training data, and its performance is evaluated on the unseen testing data.
- **Model Training**: The linear regression algorithm was trained on the prepared dataset to learn the coefficients for each feature.

### 3. Model Evaluation & Interpretation

The model's performance was assessed using standard regression metrics:
- **R-squared (R²)**: The model achieved an R-squared value of approximately **0.65**, indicating that it can explain about 65% of the variability in house prices.
- **MAE & MSE**: The Mean Absolute Error and Mean Squared Error were calculated to quantify the model's prediction accuracy.

The model's coefficients were also analyzed to determine the impact of each feature on the final price. For example, features like **area**, **bathrooms**, and having **air conditioning** were found to be significant positive predictors of a house's price.

---

## How to Run the Code

1.  Ensure you have Python and Jupyter Notebook installed.
2.  Clone this repository to your local machine.
3.  Install the required libraries:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```
4.  Open and run the Jupyter Notebook to see the full analysis.

---

## Libraries Used
- **pandas**
- **numpy**
- **scikit-learn**
- **matplotlib**
- **seaborn**
