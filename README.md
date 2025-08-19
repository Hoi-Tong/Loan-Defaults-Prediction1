# Loan Defaults Prediction

## Project Overview

This repository contains a machine learning project focused on predicting whether a loan will be defaulted upon or fully paid. The project utilizes a dataset from a lending club to build and evaluate predictive models.

The primary goal of this project is to develop a robust classification model that can accurately predict the `loan_status` of a loan application. This is a crucial task for financial institutions as it helps in risk assessment and making informed lending decisions. The project involves a complete machine learning workflow, including:

* **Exploratory Data Analysis (EDA)**: A detailed analysis of the dataset to understand its structure, identify missing values, and visualize the relationships between different features.
* **Data Preprocessing and Feature Engineering**: Cleaning the data, handling categorical variables, and engineering new features to improve model performance.
* **Model Training**: Training several machine learning models, including a **Random Forest Classifier**, to predict loan default.
* **Evaluation**: Assessing the model's performance using appropriate metrics like a confusion matrix, classification report, and ROC curve.
* **Imbalanced Data Handling**: Addressing the class imbalance in the dataset, which is a common issue in fraud and default prediction, using techniques like **Random Over-sampling**.

## Dataset

The dataset used in this project is `lending_club_loan_two.csv`, which contains various features related to loan applications, such as `loan_amnt`, `int_rate`, `emp_length`, and `annual_inc`. The target variable is `loan_status`, which is transformed into a binary `is_default` variable (1 for 'Charged Off' and 0 for 'Fully Paid').

## Technologies Used

* **Python**: The core programming language for the project.
* **Jupyter Notebook**: The primary environment for development, allowing for a clear and organized workflow.
* **Pandas**: Used for data manipulation and analysis.
* **NumPy**: Essential for numerical operations.
* **Matplotlib & Seaborn**: Libraries for data visualization and plotting.
* **Scikit-learn**: A powerful machine learning library used for building and evaluating models.
* **imblearn**: Used for handling imbalanced datasets.

## Getting Started

### Prerequisites

To run this project, you will need to have Python installed along with the following libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imblearn
```

### Usage

1.  Clone this repository:
    ```bash
    git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
    ```
2.  Navigate to the project directory:
    ```bash
    cd your-repository-name
    ```
3.  Ensure the `lending_club_loan_two.csv` dataset is present in the same directory.
4.  Open the Jupyter notebook `predict loan default.ipynb` and run all the cells to see the complete analysis and model training process.

## Results

The final model, a **Random Forest Classifier**, demonstrates promising results in predicting loan defaults. The notebook includes a detailed evaluation of its performance on the test set, including a classification report and a confusion matrix to show its predictive accuracy for both 'Fully Paid' and 'Charged Off' loans. The use of **Random Over-sampling** helped to improve the model's ability to identify the minority class (loan defaults).
