# 🏦 Bank Customer Churn Prediction

## 📌 Objective
Build a **neural network-based classifier** that can predict whether a bank customer will leave (churn) or stay with the bank in the next 6 months.

---

## 📝 Context
Customer churn is one of the most critical challenges faced by service-based businesses such as banks.  
Understanding **why customers leave** and **which factors influence their decision** allows management to take preventive actions and improve customer retention strategies.  

This project leverages machine learning—specifically a **neural network model**—to identify patterns in customer behavior and predict churn probability.

---

## 📂 Dataset
- **Source**: [Kaggle - Bank Customer Churn Modeling](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)  
- **Size**: 10,000 records × 14 features  

### 🔑 Data Dictionary
| Feature          | Description |
|------------------|-------------|
| RowNumber        | Row number (index) |
| CustomerId       | Unique identifier for each customer |
| Surname          | Customer’s surname |
| CreditScore      | Numerical measure of customer’s creditworthiness (300–900) |
| Geography        | Customer’s country |
| Gender           | Male/Female |
| Age              | Age of the customer |
| Tenure           | Number of years customer has been with the bank |
| Balance          | Account balance |
| NumOfProducts    | Number of products the customer has with the bank |
| HasCrCard        | Whether the customer owns a credit card (1 = Yes, 0 = No) |
| IsActiveMember   | Whether the customer is considered active |
| EstimatedSalary  | Estimated salary of the customer |
| Exited           | Target variable → 1 if customer left the bank, else 0 |

---

## ⚙️ Methodology
1. **Data Preprocessing**
   - Handling categorical features (encoding)
   - Normalization of numerical values
   - Train/Validation/Test split  

2. **Model Development**
   - Neural Network architecture using Keras/TensorFlow  
   - Layers: Input → Hidden Dense layers (ReLU) → Output (Sigmoid)  
   - Optimizer: Adam  
   - Loss Function: Binary Crossentropy  

3. **Evaluation**
   - Metrics: Accuracy, Loss (Train, Validation, Test)  
   - Visualizations: Loss/Accuracy curves  

---

## 📊 Results
| Dataset    | Accuracy | Loss   |
|------------|----------|--------|
| Train      | 86.56%   | 0.334  |
| Validation | 86.88%   | 0.348  |
| Test       | 84.11%   | 0.386  |

✅ The model generalizes well with only a small drop from training to test accuracy.  

---

## 🚀 Future Enhancements
- Hyperparameter tuning (learning rate, batch size, dropout, layers)  
- Experiment with advanced architectures (CNNs on embeddings, RNNs, Transformers)  
- Apply **SHAP/Feature Importance** for explainability  
- Deploy using **Streamlit/Flask** for an interactive churn prediction app  

---

## 📌 How to Run
1. Clone this repo:
   ```bash
   git clone https://github.com/Ashish152003/bank_customer_churn_prediction.git
