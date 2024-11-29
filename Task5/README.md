# Credit Card Fraud Detection

This project focuses on detecting fraudulent credit card transactions using machine learning techniques. Given the highly imbalanced nature of the dataset, the notebook employs effective data preprocessing methods and model evaluation strategies to achieve robust performance.

## Project Overview

Credit card fraud is a growing concern in the financial sector. This project addresses the challenge of identifying fraudulent transactions from a dataset containing anonymized transaction records. It utilizes oversampling methods to balance the dataset and trains a classification model to accurately distinguish between legitimate and fraudulent transactions.

## Features

1. **Data Preprocessing**:
   - Handling imbalanced data using **SMOTE (Synthetic Minority Oversampling Technique)**.
   - Exploring and scaling features as needed.

2. **Exploratory Data Analysis (EDA)**:
   - Visualizations to understand data distribution and feature importance.

3. **Machine Learning Pipeline**:
   - Logistic Regression is used as the baseline model.
   - Splitting the dataset into training and testing subsets for validation.

4. **Model Evaluation**:
   - Use of metrics such as confusion matrix, precision, recall, and F1-score to assess model performance.

## Dataset

The dataset contains anonymized credit card transactions. Key details:
- **Features**: Includes 28 anonymized PCA components (`V1`, `V2`, ..., `V28`), along with `Time` and `Amount`.
- **Target Variable**: `Class` (0 = legitimate, 1 = fraudulent).
- **Challenge**: A highly imbalanced dataset, with fraudulent transactions comprising a small percentage of total records.

### Data Source

The dataset is publicly available and can be downloaded from [Kaggle's Credit Card Fraud Detection dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud).

## Project Workflow

1. **Data Loading**:
   - Importing and inspecting the dataset using `pandas`.
   
2. **Exploratory Data Analysis (EDA)**:
   - Analyzing class distribution and feature correlations.

3. **Data Preprocessing**:
   - Splitting data into training and test sets.
   - Applying **SMOTE** to oversample the minority class.

4. **Model Training**:
   - Logistic Regression is trained on the preprocessed dataset.

5. **Model Evaluation**:
   - Evaluating model performance using classification metrics.

## Prerequisites

Ensure the following Python libraries are installed:
- `pandas`
- `numpy`
- `scikit-learn`
- `imbalanced-learn`
- `matplotlib`

Install dependencies using the following command:
```bash
pip install pandas numpy scikit-learn imbalanced-learn matplotlib
```

## How to Use

1. Clone this repository or download the notebook (`Credit_Card_Fraud_Detection.ipynb`).
2. Place the dataset (`creditcard.csv`) in the project directory.
3. Open the notebook in Jupyter Notebook or Jupyter Lab.
4. Follow the notebook cells to:
   - Preprocess the data.
   - Train the Logistic Regression model.
   - Evaluate the model's performance.

## Results

- **Before SMOTE**: The model struggles to identify fraudulent transactions due to class imbalance.
- **After SMOTE**: The model achieves improved recall and F1-score, indicating better detection of fraud.

## Future Enhancements

- Experimenting with more advanced algorithms like Random Forest, Gradient Boosting, or Neural Networks.
- Incorporating additional feature engineering techniques.
- Exploring real-time fraud detection systems.

## License

This project is licensed under the MIT License. Feel free to use, modify, and distribute as needed.
