# 📊 Customer Churn Prediction Using Artificial Neural Networks (ANN)

## 📌 Project Overview

Customer churn is a major challenge for businesses, especially in the banking industry. Losing customers can negatively impact revenue and long-term growth.

This project uses an **Artificial Neural Network (ANN)** built with TensorFlow and Keras to predict whether a bank customer is likely to leave the bank.

The application takes customer information as input, processes the data using trained preprocessing techniques, and predicts the probability of customer churn. It also provides an interactive web interface built with Streamlit.

## 🎯 Project Objectives

- Build an ANN model to predict customer churn.
- Perform data preprocessing and feature encoding.
- Apply feature scaling to prepare data for model prediction.
- Use TensorFlow and Keras to develop a deep learning model.
- Create an interactive web application using Streamlit.
- Display churn probability and the predicted customer status.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| TensorFlow | Deep learning framework |
| Keras | Building and loading the ANN model |
| Pandas | Data manipulation and preprocessing |
| NumPy | Numerical computations |
| Scikit-learn | Feature encoding and scaling |
| Pickle | Saving and loading preprocessing objects |
| Streamlit | Building the interactive web application |
| Jupyter Notebook | Experimentation and model development |

## ⚙️ Features

- **Customer Information Input:** Enter customer details through an interactive interface.
- **Geography Encoding:** Convert geographical categories into numerical features using One-Hot Encoding.
- **Gender Encoding:** Convert categorical gender values into numerical representations.
- **Feature Scaling:** Apply a trained scaler to normalize input features consistently with the model's training pipeline.
- **ANN-Based Prediction:** Use a trained artificial neural network to estimate customer churn probability.
- **Probability Display:** Display the predicted churn probability.
- **Customer Classification:** Classify customers as likely or unlikely to churn using a probability threshold of 0.5.

## 📥 Input Features

The model uses the following customer attributes to generate predictions:

| Feature | Description |
|---|---|
| CreditScore | Customer's credit score |
| Geography | Customer's geographical location |
| Gender | Customer's gender |
| Age | Customer's age |
| Tenure | Number of years the customer has been with the bank |
| Balance | Customer's bank account balance |
| NumOfProducts | Number of bank products used by the customer |
| HasCrCard | Whether the customer has a credit card |
| IsActiveMember | Whether the customer is an active bank member |
| EstimatedSalary | Customer's estimated salary |

## 🧠 Machine Learning Workflow

The project follows a machine learning workflow consisting of the following steps:

1. **Data Preparation:** Prepare customer information for model training.
2. **Data Preprocessing:** Handle categorical variables using Label Encoding and One-Hot Encoding.
3. **Feature Scaling:** Scale numerical features using a trained Scikit-learn scaler.
4. **Model Development:** Develop an Artificial Neural Network using TensorFlow and Keras.
5. **Model Training:** Train the model to learn patterns associated with customer churn.
6. **Model Serialization:** Save the trained model and preprocessing objects for reuse.
7. **Application Development:** Build a Streamlit interface to collect customer information.
8. **Prediction:** Process the input data and generate a churn probability.
9. **Classification:** Use a threshold of 0.5 to determine whether the customer is likely to churn.

## 📂 Project Structure

```text
annclassification/
│
├── app.py
├── experiments.ipynb
├── hyperparametertuningann.ipynb
├── prediction.ipynb
├── salaryregression.ipynb
│
├── model.h5
├── label_encoder_gender.pkl
├── onehot_encoder_geo.pkl
├── scaler.pkl
│
├── requirements.txt
└── README.md
```

### File Descriptions

- `app.py`: Streamlit application for customer churn prediction.
- `experiments.ipynb`: Notebook for model experimentation.
- `hyperparametertuningann.ipynb`: Notebook for ANN hyperparameter tuning.
- `prediction.ipynb`: Notebook for prediction-related experiments.
- `model.h5`: Saved trained ANN model.
- `label_encoder_gender.pkl`: Saved gender label encoder.
- `onehot_encoder_geo.pkl`: Saved geographical One-Hot Encoder.
- `scaler.pkl`: Saved feature scaler.
- `requirements.txt`: List of Python dependencies.

The `salaryregression.ipynb` notebook is also included in the repository; its relationship to the main churn prediction project is separate from the application workflow described above.

## 🚀 Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/tejussaini/annclassification.git
```

Navigate to the project directory:

```bash
cd annclassification
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment.

**Windows:**

```bash
venv\Scripts\activate
```

**Linux/macOS:**

```bash
source venv/bin/activate
```

### 3. Install Dependencies

Install the required Python packages:

```bash
pip install -r requirements.txt
```

**Compatibility note:** The requirements file specifies TensorFlow 2.15.0. Use a compatible Python environment, such as Python 3.10 or 3.11, to avoid TensorFlow installation issues.

### 4. Run the Application

Start the Streamlit application:

```bash
streamlit run app.py
```

The application will open in your browser.

## 💻 How to Use the Application

1. Launch the Streamlit application.
2. Select the customer's geography and gender.
3. Enter the customer's credit score, age, balance, and estimated salary.
4. Select the customer's tenure, number of products, credit card status, and membership activity.
5. View the predicted churn probability.
6. Check the resulting classification to determine whether the customer is likely to leave the bank.

### Example Output

```text
Churn Probability: 0.78

The customer is likely to churn.
```

*The example above is illustrative; actual predictions depend on the trained model and the selected customer information.*

## 📈 Potential Business Applications

This project demonstrates how machine learning can support customer retention strategies.

Potential applications include:

- Identifying customers who may be at risk of leaving.
- Helping banks prioritize customer retention efforts.
- Supporting data-driven customer relationship management.
- Providing insights that can inform targeted retention campaigns.

**Note:** The model produces predictions based on learned patterns. Its outputs should be evaluated against real-world outcomes before being used to make business decisions.

## 👨‍💻 Author

**Tejus Saini**

- GitHub: https://github.com/tejussaini

## 📄 License

This project is intended for educational and machine learning experimentation purposes. Add a `LICENSE` file to the repository if you want to specify formal reuse and distribution terms.