## 👨‍💻 Author

**KUMUD RATHI**
  2301010161
B.Tech Computer Science Engineering

K.R. Mangalam University

Deep Learning Assessment – 1


## 📌 Project Overview

This project develops a **Deep Neural Network (DNN)** using **PyTorch** to predict whether a student will receive college admission based on academic performance, extracurricular activities, family background, and other relevant factors.

The project includes data preprocessing, feature engineering, model training, evaluation, and model saving.

---

## 🎯 Problem Statement

To build a Deep Learning model that predicts the admission status of a student using historical admission data.

---

## 🎯 Objectives

- Predict college admission status.
- Perform data cleaning and preprocessing.
- Apply feature engineering techniques.
- Train a Deep Neural Network (DNN).
- Evaluate the model using classification metrics.
- Save the trained model for future use.

---

## 📂 Dataset

**Dataset Name:** GenZ College Admission Prediction Dataset

**Source:** User-provided dataset (`genz_college_admission_prediction.csv`)

---

## 🛠 Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- PyTorch

---

## 📊 Data Preprocessing

The following preprocessing steps were performed:

- Removed duplicate records
- Removed unnecessary columns (Student ID)
- Checked missing values
- Encoded categorical variables using LabelEncoder
- Standardized numerical features using StandardScaler
- Split dataset into Training (80%) and Testing (20%)

---

## ⚙ Feature Engineering

Feature engineering techniques applied:

- Label Encoding
- Feature Scaling (Standardization)
- Train-Test Split
- Tensor Conversion for PyTorch
- Dropout layers to reduce overfitting

---

## 🧠 Deep Neural Network Architecture

Input Layer

↓

Dense Layer (128)

↓

ReLU

↓

Dropout (0.3)

↓

Dense Layer (64)

↓

ReLU

↓

Dropout (0.2)

↓

Dense Layer (32)

↓

ReLU

↓

Output Layer (1)

↓

Sigmoid Activation

---

## 📉 Loss Function

Binary Cross Entropy Loss (BCELoss)

Reason:

- Suitable for binary classification problems.
- Measures prediction error between actual and predicted labels.

---

## 🚀 Optimizer

Adam Optimizer

Reasons:

- Adaptive learning rate
- Faster convergence
- Stable training
- Widely used for Deep Learning models

---

## 📈 Evaluation Metrics

The model is evaluated using:

- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1 Score
- Loss vs Epoch Graph

---

## 💾 Saving the Model

```python
torch.save(model.state_dict(),"AdmissionModel.pth")
```

Load the model:

```python
model.load_state_dict(torch.load("AdmissionModel.pth"))
model.eval()
```

---

## 📁 Project Structure

```
College-Admission-Prediction/
│
├── genz_college_admission_prediction.csv
├── DeepLearning_Assessment.ipynb
├── AdmissionModel.pth
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run

1. Open Google Colab.
2. Upload the notebook.
3. Upload the dataset.
4. Run all cells sequentially.
5. Train the model.
6. Evaluate performance.
7. Save the trained model.

---

## 📌 Expected Output

- Cleaned dataset
- Trained Deep Neural Network
- Accuracy score
- Confusion Matrix
- Classification Report
- Loss vs Epoch graph
- Saved model (`AdmissionModel.pth`)

---
