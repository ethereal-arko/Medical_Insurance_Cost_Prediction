# Medical Insurance Cost Prediction

## Project Overview
This project uses **Linear Regression** to estimate medical insurance charges based on demographic and lifestyle-related features.

## Dataset
The dataset contains information about age, sex, BMI, number of children, smoking status, region, and insurance charges.

- Original records: 1,338
- Records after duplicate removal: 1,337
- Missing values: None
- Input features after one-hot encoding: 8

## Technologies Used
- Python
- NumPy and Pandas
- Matplotlib and Seaborn
- Scikit-learn
- Google Colab

## Project Workflow
1. Load and inspect the dataset.
2. Check missing values and duplicate records.
3. Perform exploratory data analysis (EDA).
4. Encode categorical variables using one-hot encoding.
5. Split the data into 80% training and 20% testing sets.
6. Train a Linear Regression model.
7. Evaluate predictions using R², MAE, and RMSE.
8. Build a prediction function for new inputs.

## Model Performance

| Metric | Result |
|---|---:|
| Training R² | 0.7299 |
| Testing R² | 0.8069 |
| Testing MAE | 4,177.05 |
| Testing RMSE | 5,956.34 |

These results correspond to the project's current train-test split. The R² score indicates how much target variation the model explains relative to a mean-prediction baseline. MAE and RMSE measure prediction error in the target's units.

## Example Prediction
For an example input with age 31, female sex, BMI 25.74, zero children, non-smoker status, and southwest region, the model predicted insurance charges of **4,805.26**.

This is a model estimate, not a guaranteed insurance quote.

## Limitations and Future Improvements
- Evaluate performance using cross-validation.
- Use a preprocessing pipeline to ensure consistent encoding.
- Compare Linear Regression with Ridge, Lasso, and tree-based regression models.
- Examine residuals and possible nonlinear relationships.
- Validate inputs before using the prediction function in an application.





