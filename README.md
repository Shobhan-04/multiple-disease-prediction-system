# Multiple Disease Prediction System

An end-to-end Machine Learning application that predicts the risk of **Diabetes, Heart Disease, and Parkinson's Disease** using patient health and clinical parameters. The system uses trained classification models and provides predictions through an interactive **Streamlit** web interface.

## 🚀 Features

* **Diabetes Prediction** using Support Vector Machine (SVM)
* **Heart Disease Prediction** using Logistic Regression
* **Parkinson's Disease Prediction** using Support Vector Machine (SVM)
* Data preprocessing and feature scaling
* Model-based risk prediction using clinical parameters
* Unified Streamlit interface for all three prediction tasks
* Real-time prediction results through an interactive web application

## 🧠 Machine Learning Models

| Disease             | Model                        |
| ------------------- | ---------------------------- |
| Diabetes            | Support Vector Machine (SVM) |
| Heart Disease       | Logistic Regression          |
| Parkinson's Disease | Support Vector Machine (SVM) |

The models are trained independently because each disease dataset contains different clinical features and prediction requirements.

## 🛠️ Tech Stack

* **Language:** Python
* **Data Processing:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Models:** SVM, Logistic Regression
* **Web Framework:** Streamlit
* **Development:** Jupyter Notebook / VS Code
* **Version Control:** Git & GitHub

## 📊 Machine Learning Workflow

```text
Clinical Dataset
       ↓
Data Preprocessing
       ↓
Feature Selection
       ↓
Feature Scaling
       ↓
Train/Test Split
       ↓
Model Training
       ↓
Model Evaluation
       ↓
Saved Trained Model
       ↓
Streamlit Application
       ↓
User Input → Disease Risk Prediction
```

## 📁 Project Structure

```text
multiple-disease-prediction-system/
│
├── Diabetes_Prediction/
│   ├── diabetes.csv
│   └── diabetes_prediction.ipynb
│
├── Heart_Disease_Prediction/
│   ├── heart_disease_data.csv
│   └── heart_disease_prediction.ipynb
│
├── Parkinson_Prediction/
│   ├── parkinsons.csv
│   └──  parkinsons_prediction.ipynb
│   
│
├── app.py
├── requirements.txt
└── README.md
```

> File and folder names may vary depending on the final repository structure.

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/Shobhan-04/multiple-disease-prediction-system.git
cd multiple-disease-prediction-system
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

On Linux/macOS:

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit application

```bash
streamlit run app.py
```

The application will open in your browser at the local Streamlit address.

## 📈 Model Evaluation

The individual classification models were evaluated using standard machine-learning evaluation techniques after preprocessing and feature scaling.

The implemented models achieved approximately **95–97% accuracy** on their respective evaluation datasets.

> **Note:** Accuracy values are dataset- and split-dependent and should not be interpreted as clinical diagnostic accuracy.

## 🖥️ Application

The Streamlit application provides a unified interface where users can select a disease prediction module and enter the corresponding clinical parameters.

```text
┌─────────────────────────────────────┐
│     Multiple Disease Prediction     │
├─────────────────────────────────────┤
│                                     │
│  Select Prediction:                 │
│  • Diabetes                         │
│  • Heart Disease                   │
│  • Parkinson's Disease              │
│                                     │
│  Enter Clinical Parameters          │
│             ↓                       │
│      Generate Prediction            │
│             ↓                       │
│       Display Result                │
│                                     │
└─────────────────────────────────────┘
```

## 🔬 Disease Prediction Modules

### Diabetes Prediction

Uses patient health parameters associated with diabetes risk and applies an **SVM classifier** to generate the prediction.

### Heart Disease Prediction

Uses relevant cardiovascular and clinical parameters and applies **Logistic Regression** for binary classification.

### Parkinson's Disease Prediction

Uses voice-related biomedical features from the Parkinson's dataset and applies an **SVM classifier** for prediction.

## 📚 Key Concepts Demonstrated

* Supervised Machine Learning
* Binary Classification
* Support Vector Machines
* Logistic Regression
* Feature Scaling
* Data Preprocessing
* Model Evaluation
* Multiple Independent ML Pipelines
* Streamlit Application Development
* Model Deployment

## ⚠️ Disclaimer

This project is developed for **educational and demonstration purposes only**. It is not intended to provide medical diagnosis, treatment recommendations, or clinical decision-making. Predictions generated by the application should not be considered a substitute for professional medical advice.

## 👨‍💻 Author

**Shobhan Satpathy**

* GitHub: https://github.com/Shobhan-04
* LinkedIn: https://www.linkedin.com/in/shobhanengineer
* LeetCode: https://leetcode.com/u/SHOBHAN_04/

## ⭐ Future Improvements

* Add probability/confidence visualization for predictions
* Improve model evaluation using cross-validation
* Add additional disease prediction modules
* Introduce explainable AI techniques such as SHAP
* Build a dedicated frontend and backend architecture
* Add automated model training and evaluation pipelines

---

If you find this project useful, consider giving the repository a ⭐ on GitHub.
