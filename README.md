# Medical Insurance Cost Prediction Using KNN Regression

## Project Overview

Medical insurance charges vary from person to person depending on several factors, including age, gender, BMI, number of children, smoking habits, and residential region.

This project uses **K-Nearest Neighbors (KNN) Regression**, a Machine Learning algorithm, to predict medical insurance charges based on individual characteristics and lifestyle factors.

The model identifies similar individuals from historical data and uses their insurance charges to estimate costs for new individuals.

## Problem Definition

The objective is to develop a Machine Learning model using KNN Regression to predict an individual's medical insurance charges based on personal and lifestyle factors.

**Goal:** Predict medical insurance charges and understand how KNN Regression can be used for cost estimation.

## Dataset Information

The project uses `insurance.csv`.

| Feature | Description |
|---|---|
| age | Age of the individual |
| sex | Gender |
| bmi | Body Mass Index |
| children | Number of children |
| smoker | Smoking status |
| region | Residential region |
| charges | Medical insurance charges (Target) |

- Initial dataset records: 1,338
- Records after duplicate removal: 1,337
- Total columns: 7
- Missing values: 0
- Duplicate records removed: 1

## Technologies & Libraries

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. Data Collection
2. Data Loading
3. Data Cleaning
4. Data Understanding
5. Feature Selection
6. Categorical Data Encoding (One-Hot Encoding)
7. Train-Test Splitting
8. Feature Scaling (StandardScaler)
9. Model Building (KNN Regression)
10. Model Training
11. Prediction
12. Model Evaluation
13. New Data Prediction

## Machine Learning Algorithm

**K-Nearest Neighbors (KNN) Regression**

KNN Regression predicts a continuous numerical value by identifying the nearest data points to a new input and calculating an estimate based on their target values.

Model configuration:
- Algorithm: KNeighborsRegressor
- Number of Neighbors (K): 5
- Training Data: 80%
- Testing Data: 20%
- Random State: 42
- Scaling Technique: StandardScaler

## Model Evaluation

The model was evaluated using four regression metrics.

| Evaluation Metric | Result |
|---|---:|
| MAE | 3,494.66 |
| MSE | 30,343,819.73 |
| RMSE | 5,508.52 |
| R² Score | 0.8349 |

**R² Score: 0.8349**

The model achieved an R² score of approximately 83.49% on the test dataset.

## Sample Prediction

The trained model was tested with a new individual's information.

| Feature | Input |
|---|---|
| Age | 29 |
| Gender | Female |
| BMI | 26.5 |
| Children | 1 |
| Smoker | No |
| Region | Southeast |

**Predicted Insurance Charges: 6,786.76**

## Key Learnings

- Understanding the Machine Learning regression workflow.
- Handling missing values and duplicate records.
- Converting categorical variables using One-Hot Encoding.
- Understanding the importance of feature scaling in KNN.
- Training and testing a KNN Regression model.
- Evaluating model performance using regression metrics.
- Making predictions on new data.

## Project Files

- `KNN(regression).ipynb` – Jupyter Notebook containing the complete implementation.
- `insurance.csv` – Dataset required to execute the notebook.

## How to Run the Project

1. Clone this repository.
2. Install the required Python libraries.
3. Place `insurance.csv` in the same directory as the notebook.
4. Open the notebook using Jupyter Notebook.
5. Run the cells sequentially to perform preprocessing, model training, evaluation, and prediction.

Install dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

## Conclusion

This project demonstrates how KNN Regression can be applied to medical insurance cost prediction using individual and lifestyle-related features.

The model achieved an R² score of 0.8349, demonstrating its ability to estimate insurance charges on the test dataset.

This project helped strengthen my understanding of data preprocessing, feature encoding, feature scaling, regression modeling, and model evaluation.

---

**Project Type:** Supervised Machine Learning – Regression

**Algorithm:** K-Nearest Neighbors (KNN) Regression
