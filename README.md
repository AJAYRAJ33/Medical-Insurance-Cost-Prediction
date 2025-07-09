# 💸 Insurance Cost Prediction App

This is a machine learning project that predicts a person's insurance charges based on their demographic and lifestyle features like age, sex, BMI, number of children, smoking status, and region.

## 📊 Features

- Predicts insurance cost using a trained `LinearRegression` model
- Accepts user input in numeric format during cell execution
- Preprocesses categorical data using Label Encoding
- Trained on a dataset with features:
  - `age`, `sex`, `bmi`, `children`, `smoker`, `region`

## 📁 Project Structure
.
├── insurance_model.ipynb # Jupyter notebook with model training and prediction
├── insurance.csv
├── README.md
└── requirements.txt


## 🚀 How to Run

1. Clone this repo:

```bash
git clone https://github.com/your-username/insurance-cost-prediction.git
cd insurance-cost-prediction

2. Install dependencies:
pip install -r requirements.txt


3. Run the notebook:
jupyter notebook insurance_model.ipynb

4. Enter inputs when prompted in the notebook:
Age: 45
Sex (0 = female, 1 = male): 1
BMI: 28.5
Children: 2
Smoker (0 = yes, 1 = no): 0
Region (0 = southeast, 1 = southwest, 2 = northeast, 3 = northwest): 1


Output
✅ Estimated insurance cost (USD): 16542.87


Preprocessing
Categorical columns sex, smoker, region are label-encoded.
No NaN values are allowed during prediction.
Column order during prediction must match training order:
['age', 'sex', 'bmi', 'children', 'smoker', 'region']