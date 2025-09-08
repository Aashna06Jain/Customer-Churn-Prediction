# Customer-Churn-Prediction
This project predicts **customer churn** (whether a bank customer will leave) using a **Machine Learning model** built with Python. The project emphasizes data preprocessing, model building, and evaluation, with a simple **Flask-based interface** for demonstration.

## ✨ Features

### 🔹 Data Preprocessing
- Detect and summarize **missing values**
- Remove irrelevant columns: `RowNumber`, `CustomerId`, `Surname`
- Encode categorical variables:
  - `Geography` → one-hot encoding (France, Spain, Germany)
  - `Gender` → one-hot encoding (Male/Female)
- Scale numerical features using **StandardScaler**

### 🔹 Model Building
- **Neural Network (MLPClassifier)** with:
  - Two hidden layers: **64 neurons** and **32 neurons**
  - Activation function: **ReLU**
  - Optimizer: **Adam**
  - Learning rate: **0.01**
  - **Early stopping** enabled (stops training if no improvement)
  - Regularization parameter **alpha = 0.001**

### 🔹 Model Evaluation
- Accuracy score on test data
- Detailed **classification report** (Precision, Recall, F1-score)
- Churn distribution statistics:
  - Total customers
  - Number of churned customers
  - Number of non-churned customers
  - Churn rate

### 🔹 Model Persistence
- Save trained model as **`model.pkl`**
- Save fitted scaler as **`scaler.pkl`**

### 🔹 (Optional) Flask Web App
- Simple **UI form (`index.html`)** for entering customer details
- Displays churn **prediction**:
  - `0 = stays`
  - `1 = churns`
- Shows churn **probability score**

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
```

### 2. Install dependencies
```bash
pip install pandas numpy scikit-learn flask
```

### 3. Train the model
```bash
python model.py
```

### 4. Start the flask app
```bash
python main.py
```

## Author
- Aashna Jain
- GitHub Profile => https://github.com/Aashna06Jain
