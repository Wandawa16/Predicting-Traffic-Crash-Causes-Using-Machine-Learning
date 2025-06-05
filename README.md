#  Traffic Crash Cause Prediction

This project uses machine learning to predict the **primary contributory cause** of traffic crashes. By analyzing real-world crash data, the model helps inform road safety strategies for government agencies and transportation authorities.

---

##  Business Objective

- Predict the **primary cause** of a traffic crash.
- Help policy makers and traffic safety agencies **allocate resources efficiently**.
- Reduce crash rates through **data-driven insights**.

---

##  Data Cleaning

- Removed duplicate records.
- Handled missing values in key columns (e.g., weather conditions, road surface).
- Filtered out irrelevant columns with too many nulls or low variance.
- Converted date/time columns into usable datetime objects.
- Standardized categorical values (e.g., uppercase/lowercase mismatches).

---

##  Feature Engineering

- Extracted day of week, hour of day from crash timestamp.
- Grouped rare categories in features like `weather_condition` and `traffic_control_device`.
- One-hot encoded categorical features for model compatibility.
- Scaled/normalized numerical features (where needed).
- Dropped target leakage variables (e.g., post-crash outcomes like injuries/fatalities).

---

##  Machine Learning Models Used

-  **Random Forest Classifier** *(Best Performance)*  
- XGBoost  
- Decision Tree  
- Logistic Regression  

---

##  Model Performance

| Model              | Accuracy | F1 Score |
|-------------------|----------|----------|
| **Random Forest** | 96.8%    | 0.9677   |
| XGBoost           | 95.7%    | 0.9571   |
| Decision Tree     | 91.4%    | 0.9136   |
| Logistic Regression | 55.2%  | 0.5325   |

---

## Evaluation Metrics

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  
- Classification Report  

---

##  Project Structure
data/ # Raw ,cleaned datasets and predictions.csv 
├──  Jupyter notebooks for EDA & modeling
├── visuals/ # Charts, graphs, and plots
├── README.md # Project overview and instructions


