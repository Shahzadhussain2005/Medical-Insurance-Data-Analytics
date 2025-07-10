# 🩺 Medical Insurance Charges Prediction

This project aims to predict individual medical insurance charges based on various health and demographic 
factors using data analytics and machine learning techniques. The workflow includes data cleaning, 
exploratory data analysis (EDA), model development using pipelines, and model refinement with Ridge regression and polynomial transformation.

---

## 📁 Dataset

The dataset contains the following features:

- `age`: Age of the primary beneficiary
- `sex`: Gender of the beneficiary
- `bmi`: Body Mass Index
- `children`: Number of dependents covered by insurance
- `smoker`: Smoking status (`yes`/`no`)
- `region`: Residential region in the U.S.
- `charges`: Medical insurance charges (target variable)

---

## 🛠️ Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib & Seaborn (for visualization)
- Scikit-learn (`sklearn`)

---

## 📊 Project Workflow

### 1. **Data Loading and Cleaning**
- Imported the dataset using Pandas.
- Handled missing values (if any).
- Cleaned and formatted data types for modeling.

### 2. **Exploratory Data Analysis (EDA)**
- Visualized distributions of key features like age, BMI, and charges.
- Explored relationships between predictors and target variable (`charges`).
- Investigated the influence of smoking and BMI on insurance charges.

### 3. **Feature Engineering**
- Encoded categorical variables such as `sex` and `smoker`.
- Built preprocessing pipelines using `StandardScaler` and `ColumnTransformer`.

### 4. **Model Development**
- Initially built a simple linear regression model using only `BMI` to predict charges.
- Extended the model to include all features (`age`, `sex`, `bmi`, `children`, `smoker`, `region`).

### 5. **Model Refinement**
- Split the dataset into training and testing sets using `train_test_split`.
- Applied **Ridge Regression** with `alpha=0.1` to reduce overfitting.
- Performed **polynomial feature transformation** with `degree=2` to capture non-linear relationships.

---

## 🔍 Results

- Evaluated models using **R² Score** to assess performance.
- Ridge Regression with polynomial features improved predictive accuracy over simple linear models.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yShahzadhussain2005/Medical-Insurance-Data-Analytics-ML.git
   cd Medical-Insurance-Data-Analytics-ML
   Install the required libraries:

bash

pip install -r requirements.txt
Run the main notebook or script:

jupyter notebook

📌 Future Work
Hyperparameter tuning using GridSearchCV.

Try other models like Lasso Regression, Decision Trees, or Gradient Boosting.

Deploy the model as a web app using Flask or Streamlit.
