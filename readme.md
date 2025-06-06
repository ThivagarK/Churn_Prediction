## Customer Churn Prediction Web App
A binary classification project to predict whether a bank customer is likely to churn (discontinue service) based on customer demographics and account behavior. Built using TensorFlow, Scikit-learn, and deployed using Streamlit.

## Problem Statement
Churn prediction helps banks and financial institutions identify customers who are likely to leave. This tool uses a trained neural network to provide real-time churn probability for any customer profile.

## Features
🧠 Deep Learning Model with dropout layers and optimizers

🛠 Standardization & encoding of input features

📁 Model and preprocessing artifacts stored as .h5 and .pkl

🌐 User-friendly interface via Streamlit

☁️ Easily deployable to Streamlit Cloud

## Tech Stack
| Tool                   | Purpose                                                   |
| ---------------------- | --------------------------------------------------------- |
| `TensorFlow / Keras`   | Build and train the neural network                        |
| `Scikit-learn	`        | Preprocessing (Scaling, Label Encoding, One-Hot Encoding) |
| `Pandas / NumPy`       | Data handling                                             |
| `Streamlit`            | Web app interface                                         |
| `Pickle`               | Store encoders and scaler                                 |

🚀 How to Run the App
1. Clone the repository
```bash
git clone https://github.com/yourusername/churn-predictor.git
cd churn-predictor
```
2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Make sure the following files are present:
model.h5
scaler.pkl
label_encoder_gender.pkl
onehot_encoder_geo.pkl

4. Run the Streamlit app
```bash
streamlit run app.py
```

## Model Inputs
```
Feature	Description
Geography	Country/Region (one-hot encoded)
Gender	Male/Female (label encoded)
Age	Customer age
Credit Score	Creditworthiness
Balance	Bank balance
Estimated Salary	Annual income estimate
Tenure	Years with the bank
Num of Products	Number of products owned
Has Credit Card	Whether the customer has a credit card
Is Active Member	Whether the customer is active
```

## 🧠 Output
Churn Probability (e.g., 0.76)

Prediction Message:
The customer is likely to churn.
The customer is not likely to churn.

## 📌 Future Improvements
1. Add visual analytics (charts, SHAP explainability)

2. Support CSV uploads for bulk predictions

3. Include historical churn rate tracking
