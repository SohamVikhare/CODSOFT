# Titanic Survival Prediction

## Overview of `Titanic_Prediction.ipynb`

This Jupyter Notebook provides a comprehensive analysis and predictive modeling of Titanic passenger survival data. It is structured to guide users through data analysis, preprocessing, and machine learning techniques to predict whether a passenger survived based on their attributes.

## Workflow Overview

1. **Introduction**
   - Provides context and objectives for the Titanic prediction task.

2. **Data Loading**
   - Loads the Titanic dataset into a pandas DataFrame for analysis.
   - Dataset inspection includes examining its structure, summary statistics, and identifying missing values.

3. **Exploratory Data Analysis (EDA)**
   - Visualizations and statistical analyses reveal survival patterns by features such as:
     - Gender
     - Passenger class (Pclass)
     - Age groups
   - Tools used: `seaborn` and `matplotlib`.

4. **Data Preprocessing**
   - Missing values are handled for critical columns like `Age` and `Embarked`.
   - Encoding categorical variables (e.g., `Sex`, `Embarked`) into numeric formats.
   - Features such as `Fare` are scaled for uniformity.

5. **Model Training**
   - Implements several machine learning algorithms:
     - Logistic Regression
     - Decision Trees
     - Random Forest
   - Models are trained and validated using scikit-learn.

6. **Model Evaluation**
   - Metrics such as accuracy, precision, recall, and F1-score assess the models' performance.
   - Visualizations compare the effectiveness of different algorithms.

7. **Conclusion**
   - Summarizes findings and offers suggestions for further improvements.

## Dataset Details

The Titanic dataset, sourced from [Kaggle](https://www.kaggle.com/c/titanic/data), contains information about passengers, including:

- **Pclass**: Ticket class (1st = highest, 3rd = lowest)
- **Sex**: Gender of the passenger
- **Age**: Age of the passenger
- **SibSp**: Number of siblings or spouses aboard
- **Parch**: Number of parents or children aboard
- **Fare**: Ticket price
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
- **Survived**: Target variable (0 = Did not survive, 1 = Survived)

### Data Preprocessing Highlights
- **Handling Missing Values:**
  - Median imputation for `Age`.
  - Mode imputation for `Embarked`.
- **Encoding:**
  - `Sex` and `Embarked` converted to numerical categories.
- **Feature Scaling:**
  - Applied to `Fare` for consistent input.

## How to Run the Notebook

1. **Environment Setup:**
   - Install required libraries using:
     ```bash
     pip install pandas numpy matplotlib seaborn scikit-learn
     ```

2. **Open the Notebook:**
   - Launch Jupyter Notebook and open `Titanic_Prediction.ipynb`.

3. **Execute Cells Sequentially:**
   - Follow the notebook structure, executing cells in order for smooth reproducibility.

## Purpose of the Notebook
This notebook is ideal for:
- Beginners learning data science and machine learning workflows.
- Practitioners exploring binary classification problems.
- Educators teaching predictive modeling techniques.

Feel free to explore, modify, and improve upon the work provided in this notebook.

