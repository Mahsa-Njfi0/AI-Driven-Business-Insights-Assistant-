AI‑Driven Business Insights Assistant
This project builds a full AI/ML pipeline to predict customer churn using a real‑world CRM dataset from a telecommunications provider.
It demonstrates the complete lifecycle of an AI solution:

Data cleaning & preprocessing

Feature engineering

Model development using scikit‑learn, TensorFlow, and PyTorch

Model evaluation & comparison

Business‑focused interpretation

Documentation of findings and next steps

This project aligns with real industry workflows and showcases practical AI engineering skills.

Project Structure

ai-business-insights-assistant/
│
├── data/
│   └── crm/
│       └── telco_churn.csv
│
├── notebooks/
│   └── 01_crm_eda.ipynb
│
├── models/
│   ├── logistic_regression.pkl
│   ├── random_forest.pkl
│   ├── xgboost_model.pkl
│   ├── tensorflow_model.h5
│   └── pytorch_model.pt
│
├── README.md
└── requirements.txt

-------------------------------------------------------------------

📊 Dataset
The CRM dataset contains customer demographic information, service usage, billing details, and churn labels.

Rows: 7,043

Columns: 21

Target: Churn (Yes/No)

Key challenges addressed:

TotalCharges stored as text

Missing values

Highly imbalanced target variable

Many categorical features requiring encoding

🧹 Data Cleaning & Preprocessing
Steps performed:

Converted TotalCharges to numeric

Removed rows with missing values

One‑hot encoded categorical variables

Scaled features for neural networks

Stratified train/test split

Applied class weighting to handle imbalance

---------------------------------------------------------------

🤖 Models Developed
1. Classical ML Models (scikit‑learn)
Logistic Regression

Random Forest

XGBoost

Each model was trained, evaluated, and compared using:

Accuracy

Precision

Recall

F1‑score

Confusion matrix

2. Deep Learning Model (TensorFlow/Keras)
A fully connected neural network with:

Dense layers

ReLU activation

Dropout regularization

Sigmoid output

Trained for 30 epochs with validation monitoring.

3. Deep Learning Model (PyTorch)
A custom neural network built using:

nn.Linear layers

ReLU activation

Dropout

Adam optimizer

Manual training loop with DataLoader

This demonstrates low‑level deep learning proficiency.

----------------------------------------------------------------

📈 Model Comparison
Model	Library	Accuracy	Recall (Churn=1)	Precision (Churn=1)	F1‑Score (Churn=1)
Logistic Regression	scikit‑learn	0.72	0.80	0.49	0.61
Random Forest	scikit‑learn	0.79	0.51	0.63	0.56
XGBoost	XGBoost	0.75	0.72	0.53	0.61
Neural Network	TensorFlow	0.78	0.31	0.71	0.43
Neural Network	PyTorch	0.73	0.00	0.00	0.00

----------------------------------------------------------------------

📝 Project Summary
This project demonstrates the full lifecycle of an AI solution for churn prediction, including EDA, data cleaning, feature engineering, classical ML models, and deep learning models using TensorFlow and PyTorch.
It highlights practical experience with CRM data, model evaluation, and cross‑framework development — key skills for an AI Engineer role.

----------------------------------------------------------------------------------

🚀 Next Steps
Hyperparameter tuning (Grid Search, Optuna)

SMOTE or focal loss for imbalance

SHAP/LIME explainability

Deployment via API or Streamlit

Monitoring for data/model drift

---------------------------------------------------------------------------------------

🛠️ Technologies Used
Python

pandas, NumPy

scikit‑learn

XGBoost

TensorFlow / Keras

PyTorch

Matplotlib / Seaborn

------------------------------------------------------------------------------------------

📬 Contact
If you’d like to discuss this project or collaborate, feel free to reach out.