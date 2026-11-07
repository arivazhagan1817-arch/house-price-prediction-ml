# House Price Prediction using Machine Learning

## Project Overview
This project focuses on predicting house prices using supervised machine learning regression algorithms. It uses the Ames Housing dataset and compares multiple regression models to identify the best-performing model.

## Dataset
- Dataset: Ames Housing Dataset
- Source: OpenML (Data ID: 42165)
- Total records: 1,460
- Target variable: `SalePrice`

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Joblib
- Jupyter Notebook

## Project Workflow
1. Loaded and explored the dataset.
2. Handled missing values using SimpleImputer.
3. Applied StandardScaler to numerical features.
4. Applied OneHotEncoder to categorical features.
5. Built preprocessing and machine learning pipelines.
6. Split the dataset into training and testing sets.
7. Trained and evaluated four regression models.
8. Used 5-fold cross-validation.
9. Applied GridSearchCV for hyperparameter tuning.
10. Compared model performance and selected the best model.

## Models Implemented
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- Tuned Gradient Boosting Regressor

## Model Comparison

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Tuned Gradient Boosting | 16357.56 | 27245.39 | 0.9032 |
| Gradient Boosting | 16824.92 | 27725.66 | 0.8998 |
| Random Forest | 17750.58 | 29350.90 | 0.8877 |
| Linear Regression | 18362.24 | 29445.76 | 0.8870 |
| Decision Tree | 28882.77 | 44841.58 | 0.7379 |

## Hyperparameter Tuning
GridSearchCV with 5-fold cross-validation was used to tune the Gradient Boosting Regressor.

**Best Parameters:**
- Learning Rate: 0.1
- Max Depth: 3
- Number of Estimators: 200

## Best Model Performance

**Tuned Gradient Boosting Regressor**

- MAE: 16,357.56
- RMSE: 27,245.39
- R² Score: 0.9032 (90.32%)

The tuned Gradient Boosting model achieved the best results among the evaluated models.

## Project Files
- `Supervised_Regression_Modeling_Tuning.ipynb` – Complete model training, evaluation, and tuning workflow.
- `best_house_price_model.joblib` – Saved trained model pipeline.
- `requirements.txt` – Required Python libraries.

## How to Run
1. Clone this repository.
2. Install the required dependencies:
   `pip install -r requirements.txt`
3. Open the Jupyter Notebook.
4. Run the cells to explore the workflow and results.

## Conclusion
This project demonstrates a complete supervised regression workflow, including data preprocessing, model training, cross-validation, hyperparameter tuning, and model evaluation. Tuned Gradient Boosting achieved the best performance with an R² score of 0.9032.

---
**Project Type:** Machine Learning – Supervised Regression
