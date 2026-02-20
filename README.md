# Diabetes Risk Prediction using Artificial Neural Network (ANN)

## 📌 Project Overview
This project develops a binary classification model to predict whether a patient is likely to have diabetes based on medical diagnostic measurements.

A feedforward Artificial Neural Network (ANN) was implemented using TensorFlow/Keras and evaluated using multiple optimizers to compare performance.

---

## 📊 Dataset
- Source: Pima Indians Diabetes Dataset
- Total Records: 768 patients
- Features include:
  - Glucose Level
  - Blood Pressure
  - BMI
  - Insulin
  - Age
  - Skin Thickness
  - Diabetes Pedigree Function
  - Number of Pregnancies

Target Variable:
- 0 = No Diabetes
- 1 = Diabetes

---

## 🧹 Data Preprocessing
- Replaced biologically impossible zero values with NaN
- Median imputation applied for missing values
- Train-Test Split: 75% / 25%
- Feature Scaling: StandardScaler()

---

## 🧠 Model Architecture
- Input Layer
- Hidden Layer (12 neurons, ReLU activation)
- Output Layer (Sigmoid activation)

Loss Function:
- Binary Cross Entropy

Evaluation Metrics:
- Accuracy
- ROC-AUC Score

---

## ⚙️ Optimizers Compared
| Optimizer | ROC-AUC Score |
|-----------|--------------|
| Adam      | 0.83         |
| Nadam     | 0.81         |
| SGD       | 0.80         |
| FTRL      | 0.79         |

Adam optimizer achieved the best predictive performance on the test dataset.

---

## 📈 Model Performance
- Training Accuracy: ~77%
- Testing Accuracy: ~75%
- Best ROC-AUC: 0.83 (Adam)

---

## 🛠️ Technologies Used
- Python
- Pandas
- Scikit-learn
- TensorFlow / Keras
- Matplotlib
- Seaborn

---

## 📌 Future Improvements
- Hyperparameter tuning
- Cross-validation
- Feature selection
- Deployment using Flask or Streamlit

---

## 📁 Repository Structure
