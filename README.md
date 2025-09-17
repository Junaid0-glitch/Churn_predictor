# Churn Predictor

This project analyzes customer churn data from a telecom company and builds machine learning models to predict customer churn. The workflow includes data cleaning, exploratory data analysis (EDA), feature engineering, handling class imbalance, model training, and hyperparameter tuning.

## Dataset
- **File:** WA_Fn-UseC_-Telco-Customer-Churn.csv
- Contains customer information, services, account details, and churn status.

## Steps
1. **Data Import & Cleaning**
   - Load data with pandas
   - Handle missing and duplicate values
   - Convert `TotalCharges` to float
   - Drop irrelevant columns (e.g., `customerID`)
2. **Exploratory Data Analysis (EDA)**
   - Visualize distributions and relationships
   - Identify class imbalance
3. **Feature Engineering**
   - Replace string values with numeric
   - One-hot encode categorical features
   - Scale numerical features
4. **Class Imbalance Handling**
   - Use SMOTE for oversampling
5. **Model Training & Evaluation**
   - Train multiple classifiers: Random Forest, Decision Tree, XGBoost, Logistic Regression, KNN
   - Evaluate with classification report and confusion matrix
6. **Hyperparameter Tuning**
   - Use RandomizedSearchCV for XGBoost
   - Select best model and analyze feature importances

## Requirements
- Python 3.x
- pandas
- seaborn
- matplotlib
- scikit-learn
- imbalanced-learn
- xgboost

## Usage
1. Open `churn_predictor.ipynb` in Jupyter Notebook or VS Code.
2. Run cells sequentially to reproduce the analysis and modeling steps.
3. Review results and conclusions at the end of the notebook.

## Results
- The notebook provides insights into important features affecting churn.
- The best model and its accuracy are reported after hyperparameter tuning.

## Author
- Project by [Your Name]

## License
- For educational purposes only.