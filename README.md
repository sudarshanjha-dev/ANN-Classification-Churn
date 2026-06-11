# Customer Churn Prediction using Artificial Neural Network (ANN)

## Overview

This project predicts whether a bank customer is likely to leave the bank (churn) using an Artificial Neural Network (ANN) built with TensorFlow and Keras.

Customer churn prediction helps banks identify customers who are at risk of leaving and enables them to take proactive retention measures.

The model analyzes customer information such as credit score, age, balance, geography, salary, and account activity to predict the probability of churn.

---

## Problem Statement

Customer retention is a major challenge in the banking industry. Acquiring new customers is often more expensive than retaining existing ones.

The objective of this project is to build a machine learning model capable of predicting whether a customer will leave the bank based on historical customer data.

---

## Dataset

The project uses the **Churn Modelling Dataset**, which contains customer information from a bank.

### Features

| Feature | Description |
|----------|------------|
| CreditScore | Customer credit score |
| Geography | Customer's country |
| Gender | Male/Female |
| Age | Customer age |
| Tenure | Number of years with the bank |
| Balance | Customer account balance |
| NumOfProducts | Number of products used |
| HasCrCard | Whether customer owns a credit card |
| IsActiveMember | Whether customer is an active member |
| EstimatedSalary | Estimated annual salary |

### Target Variable

| Value | Meaning |
|---------|---------|
| 0 | Customer stays |
| 1 | Customer leaves (Churn) |

---

## Technologies Used

- Python
- TensorFlow / Keras
- Scikit-Learn
- Pandas
- NumPy
- Streamlit
- Pickle

---

## Project Workflow

1. Data Collection
2. Data Cleaning and Preprocessing
3. Feature Encoding
4. Feature Scaling
5. Train-Test Split
6. ANN Model Building
7. Model Training
8. Model Evaluation
9. Model Saving
10. Streamlit Deployment

---

## Data Preprocessing

The following preprocessing techniques were applied:

### Label Encoding

Used for:

- Gender

### One-Hot Encoding

Used for:

- Geography

### Feature Scaling

Used:

```python
StandardScaler
```

to normalize numerical features.

---

## ANN Architecture

```text
Input Layer
     ↓
Dense Layer (64 Neurons, ReLU)
     ↓
Dense Layer (32 Neurons, ReLU)
     ↓
Output Layer (1 Neuron, Sigmoid)
```

### Activation Functions

- ReLU
- Sigmoid

### Loss Function

```python
binary_crossentropy
```

### Optimizer

```python
adam
```

---

## Model Performance

| Metric | Score |
|---------|---------|
| Accuracy | Add Your Accuracy |
| Precision | Add Precision |
| Recall | Add Recall |
| F1 Score | Add F1 Score |
| ROC-AUC | Add ROC-AUC |

---

## Project Structure

```text
ANN-Classification-Churn/
│
├── app.py
├── Training.ipynb
├── prediction.ipynb
├── Churn_Modelling.csv
├── model.h5
├── scaler.pkl
├── ohe.pkl
├── le.pkl
├── requirements.txt
└── README.md
```

---

## Running the Project Locally

### Clone the Repository

```bash
git clone https://github.com/sudarshanjha-dev/ANN-Classification-Churn.git
```

### Navigate to Project Directory

```bash
cd ANN-Classification-Churn
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Streamlit Application

```bash
streamlit run app.py
```

---

## Sample Prediction Workflow

1. Enter customer details.
2. Data is preprocessed using saved encoders and scaler.
3. The ANN model generates a churn probability.
4. The application displays whether the customer is likely to churn.

---

## Future Improvements

- Hyperparameter tuning
- Early stopping and dropout regularization
- K-Fold Cross Validation
- Model Explainability using SHAP
- Comparison with XGBoost, Random Forest, and CatBoost
- Cloud Deployment
- CI/CD Pipeline Integration

---

## Key Learnings

Through this project, I gained hands-on experience with:

- Artificial Neural Networks (ANNs)
- Deep Learning using TensorFlow
- Data Preprocessing
- Feature Engineering
- Model Serialization
- Streamlit Application Development
- End-to-End Machine Learning Workflow

---

## Screenshots

### Streamlit Application

Add screenshots here after deployment.

```markdown
![Home Page](screenshots/home.png)

![Prediction Page](screenshots/prediction.png)
```

---

## Author

### Sudarshan Jha

Production & Industrial Engineering  
Motilal Nehru National Institute of Technology (MNNIT) Allahabad

### Connect With Me

- GitHub: https://github.com/sudarshanjha-dev
- LinkedIn: Add Your LinkedIn Profile

---

## License

This project is open-source and available under the MIT License.
