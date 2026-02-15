# Heart_Disease_Prediction
Heart disease ML assignment for BITs

❤️ Heart Disease Prediction Using Machine Learning 📌 Project Overview

This project builds and evaluates multiple Machine Learning models to predict the presence of heart disease using the UCI Heart Disease Dataset.

The application includes:

📊 Model comparison dashboard

🧠 Real-time patient risk prediction

📁 CSV-based model evaluation

📈 Performance visualization

The project is deployed using Streamlit for interactive user experience.

📂 Dataset

Dataset Name: UCI Heart Disease Dataset

Target Variable: num (Converted to binary: 0 = No Disease, 1 = Disease)

Missing values handled using Median Imputation

Categorical features encoded using Label Encoding

⚙️ Technologies Used

Python 3.11

Scikit-learn

XGBoost

Pandas & NumPy

Matplotlib & Seaborn

Streamlit

Joblib

🏗 Project Structure Heart_Disease_Prediction/ │ ├── dataset/ │ └── heart_disease_uci.csv │ ├── model/ │ ├── preprocessing.py │ ├── train_models.py │ ├── trained_models/ │ ├── logistic_model.pkl │ ├── decision_tree_model.pkl │ ├── knn_model.pkl │ ├── naive_bayes_model.pkl │ ├── random_forest_model.pkl │ ├── xgboost_model.pkl │ ├── scaler.pkl │ ├── num_imputer.pkl │ ├── feature_columns.pkl │ ├── num_columns.pkl │ └── test_data.pkl │ ├── app.py └── README.md

🧠 Models Implemented

Logistic Regression

Decision Tree

K-Nearest Neighbors (KNN)

Naive Bayes

Random Forest

XGBoost

| Model               | Accuracy   | AUC        | Precision  | Recall     | F1 Score   | MCC        |
| ------------------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| **XGBoost**         | **0.8424** | 0.8943     | 0.8411     | **0.8824** | **0.8612** | **0.6801** |
| Random Forest       | 0.8315     | **0.9170** | 0.8447     | 0.8529     | 0.8488     | 0.6586     |
| Naive Bayes         | 0.8261     | 0.8840     | 0.8365     | 0.8529     | 0.8447     | 0.6473     |
| Logistic Regression | 0.8207     | 0.8922     | 0.8350     | 0.8431     | 0.8390     | 0.6366     |
| KNN                 | 0.8261     | 0.8877     | **0.8723** | 0.8039     | 0.8367     | 0.6538     |
| Decision Tree       | 0.7391     | 0.7324     | 0.7500     | 0.7941     | 0.7714     | 0.4692     |

🏆 Best Performing Model ✅ XGBoost

Highest Accuracy

Highest F1 Score

Highest MCC

Strong Recall (important in medical prediction)

Although Random Forest achieved the highest AUC, XGBoost provided better overall balanced performance.

📈 Evaluation Metrics Explained

Accuracy → Overall correctness

AUC → Model’s ability to distinguish between classes

Precision → Correct positive predictions

Recall → Ability to detect disease cases

F1 Score → Balance between Precision and Recall

MCC → Balanced metric for binary classification

For medical diagnosis, Recall and F1 Score are especially important to reduce false negatives.

🚀 How to Run the Project 1️⃣ Install Dependencies pip install -r requirements.txt

Or manually:

pip install streamlit scikit-learn xgboost pandas numpy matplotlib seaborn joblib

2️⃣ Train Models python model/train_models.py

3️⃣ Run Streamlit App streamlit run app.py

🖥 Application Features 🔹 Prediction Dashboard

Enter patient details

Select ML model

View predicted risk with probability

🔹 Model Evaluation

Upload CSV dataset

View confusion matrix

View classification report

🔐 Medical Disclaimer

This project is for educational purposes only. It does not replace professional medical diagnosis.

👨‍💻 Author

Developed as part of a Machine Learning academic project by Bhuvesh Singh (BITSID: 2025AA05972).
