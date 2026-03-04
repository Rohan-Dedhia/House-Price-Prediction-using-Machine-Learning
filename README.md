# 🏠 House Price Prediction using Machine Learning

This project builds a machine learning pipeline to predict housing prices using the **Ames Housing Dataset** from Kaggle. The goal is to estimate house sale prices using data preprocessing, feature engineering, regression models, and ensemble learning.


## 📊 Dataset

Dataset: **Ames Housing Dataset**  
Source: Kaggle – House Prices Competition

The dataset contains **79 explanatory variables** describing residential homes in Ames, Iowa.

Examples of features include:

- Lot Area
- Overall Quality
- Year Built
- Living Area
- Garage Capacity
- Neighborhood

Target variable: SalePrice

## ⚙️ Project Workflow

1. Data Cleaning  
2. Missing Value Handling  
3. Outlier Removal  
4. Feature Engineering  
5. Categorical Encoding (One-Hot Encoding)  
6. Feature Scaling  
7. Model Training  
8. Hyperparameter Tuning  
9. Ensemble Prediction  

## 🧠 Models Used

- Linear Regression  
- Ridge Regression  
- Lasso Regression  

Hyperparameters were optimized using **GridSearchCV with cross-validation**.

## 🔧 Key Techniques

### Log Transformation

House prices are right-skewed, so the target variable was transformed: y = np.log1p(SalePrice)

Predictions were converted back using: SalePrice = np.expm1(predictions)

## 🤖 Ensemble Model

Final predictions were generated using an ensemble of: Ridge Regression + Lasso Regression

This reduced prediction variance and improved leaderboard performance.

## 📈 Results

Initial baseline score: RMSE ≈ 16224

Final model score: RMSE ≈ 13500

This represents a **~2700 RMSE improvement through preprocessing, feature engineering, and model optimization**.

## 🛠 Tech Stack

- Python  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib  
- Jupyter Notebook  

## 📂 Project Structure
house-price-prediction-kaggle
│
├── house_price_prediction.ipynb
│
├── submission_best.csv
│
├── README.md
└── requirements.txt

## 🚀 How to Run

1. Clone the repository: git clone https://github.com/yourusername/house-price-prediction-kaggle.git
2. Install dependencies: pip install -r requirements.txt
3. Download the dataset from Kaggle and place it in the project directory.
4. Run the Jupyter notebook.

## 📌 Key Learnings

- Handling missing values in real-world datasets  
- Feature engineering for regression problems  
- Regularization techniques (Ridge & Lasso)  
- Model ensembling  
- Kaggle competition workflow  

## 🔗 Author

**Rohan Dedhia**

GitHub: https://github.com/Rohan-Dedhia
