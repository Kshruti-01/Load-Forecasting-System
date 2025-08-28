# Load-Forecasting-System
The Load Forecasting System addresses the need for accurate prediction of 
electrical load across multiple lines (33kVA, 132kVA Line 3, 132kVA Line 5). 
The project involves preprocessing raw time-series data, handling missing readings through imputation, and engineering temporal features such as day of the week, month, and holidays.
Various models, including Random Forest,XGBoost, and LSTM, were trained, validated, and compared to select the best performing model. 
The system successfully forecasts load with high accuracy, enabling proactive energy management, minimizing the risk of outages, and supporting operational planning.

# Methodology
Data Collection and Understanding
• Load data was collected with a 15-minute interval for all three 
lines.
• Missing data points were identified and quantified
Data Preprocessing and Imputation
1. Handling Missing Data
• Missing values were filled using forward fill, backward fill and fill with mean, median and mode methods.
2. Cleaning
• Removed duplicate records.
Feature Engineering
 Additional temporal and categorical features were added: Day of the week, Month, Holidays, Previous Load values
Model Development
 1.Models Implemented:
• Random Forest Regressor – Captures non-linear dependencies, 
robust to overfitting.
• XGBoost Regressor – Gradient boosting for high accuracy.
• LSTM Neural Network – Captures sequential dependencies in time 
series.
2.Process:
• Data split into training (80%) and testing (20%) sets
• Hyperparameter tuning for each model.
• Evaluation metrics: RMSE, MAE, and R² score.
Model Evaluation
# Technologies used
• Python: Pandas, NumPy
• Scikit-learn: Random Forest, XGBoost
• TensorFlow/Keras: LSTM
• Matplotlib/Seaborn: Visualization
• Joblib / Pickle: Model serialization
