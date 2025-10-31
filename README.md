# Social-Network-Ads-Sale-Prediction-Using-Machine-Learning  
Predicting Sales from Social Network Ads using Machine Learning

## About  
This repository contains a machine-learning project that aims to predict whether a user will purchase a product after being shown on a social network advertisement. The code implements exploratory data analysis (EDA), preprocessing, model training, and a simple application interface.  

## Problem Statement  
Advertising on social networks is a major channel for reaching potential customers. However, identifying **which users are likely to purchase** after seeing an ad remains a key challenge.  
This project seeks to:  
- Use demographic and behaviour features of users to predict purchase decisions.  
- Provide a predictive model to help advertisers optimise ad-spend by focusing on high-conversion users.  
- Deploy the model in a lightweight application so that the prediction can be used in real-time scenarios.  

## Dataset  
The project uses the `Social_Network_Ads.csv` dataset which includes features such as:  
- User ID  
- Gender  
- Age  
- Estimated Salary  
- Purchased (target variable: 0 = No, 1 = Yes)  
You will find the dataset in the repository root.  

## Methodology  
1. Load and inspect the data; perform EDA to understand distributions, correlations and target imbalance.  
2. Preprocessing:  
   - Encode categorical values (e.g., Gender).  
   - Scale numeric features (Age, Estimated Salary).  
   - Split data into training and testing sets.  
3. Model training:  
   - Train selected ML model(s) (e.g., Logistic Regression, Random Forest) to classify user purchase behaviour.  
   - Perform hyper-parameter tuning and cross-validation if needed.  
4. Evaluation:  
   - Generate accuracy, confusion matrix, precision, recall, F1-score.  
   - Visualise decision boundaries (for 2-feature subsets) and model behaviour.  
5. Deployment:  
   - Create a simple web app (`app.py`) and front-end (`index.html`) that loads a saved model (`model.pkl`) and allows interactive prediction.  

## Usage  
To run the project locally:  
```bash
# Clone the repository  
git clone https://github.com/611noorsaeed/Social-Network-Ads-Sale-Prediction-Using-Machine-Learning.git  
cd Social-Network-Ads-Sale-Prediction-Using-Machine-Learning  

# Install dependencies  
pip install -r requirements.txt  

# Run the Jupyter notebook for model training  
jupyter notebook “Social Network Ads Sales Prediction using Machine Leanring.ipynb”  

# Or run the web app  
python app.py  
# Then open http://localhost:5000 in your browser  
