# 🏠 House Price Prediction API

A Machine Learning-powered REST API that predicts house prices based on property features.

This project uses a trained Machine Learning model and **FastAPI** to provide real-time house price predictions through a simple API.

---

## 🚀 Features

- 🏠 House Price Prediction
- 🤖 Machine Learning-based prediction
- ⚡ FastAPI REST API
- 📊 Feature-based prediction
- 🧪 Model training pipeline
- 🔍 Exploratory Data Analysis
- 💾 Serialized ML model using Joblib
- 📖 Interactive Swagger API documentation
- 🧩 Simple and modular project structure

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| FastAPI | REST API Framework |
| Scikit-learn | Machine Learning |
| Pandas | Data Processing |
| NumPy | Numerical Computing |
| Joblib | Model Serialization |
| Uvicorn | ASGI Server |

---

## 📁 Project Structure

```text
House-Prediction-API/
│
├── explore.py
├── main.py
├── train.py
├── house_features.joblib
├── .gitignore
└── README.md
```

### File Description

| File | Description |
|---|---|
| `main.py` | Contains the FastAPI application and prediction endpoint. |
| `train.py` | Contains the Machine Learning model training process. |
| `explore.py` | Used for exploring and analyzing the dataset. |
| `house_features.joblib` | Stores the feature-related information required by the prediction pipeline. |
| `house_model.joblib` | Contains the trained Machine Learning model. |

> ℹ️ The trained model file (`house_model.joblib`) is intentionally excluded from GitHub because it is approximately 144 MB, which exceeds GitHub's standard 100 MB individual file limit.

---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/atulsahu003/House-Prediction-API.git
```

### 2. Navigate to the Project
```bash
cd House-Prediction-API
```

### 3. Create a Virtual Environment
```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

**Windows**
```bash
venv\Scripts\activate
```

**macOS / Linux**
```bash
source venv/bin/activate
```

### 5. Install Dependencies
```bash
pip install fastapi uvicorn pandas numpy scikit-learn joblib
```

---

## 🤖 Machine Learning Model

The project follows a basic Machine Learning workflow:

```
Dataset
   ↓
Data Exploration
   ↓
Feature Selection / Preparation
   ↓
Model Training
   ↓
Model Serialization
   ↓
FastAPI Integration
   ↓
House Price Prediction
```

The trained model is saved using Joblib as `house_model.joblib`.

---

## 🏋️ Training the Model

If the trained model is not available locally, run:

```bash
python train.py
```

This script trains the Machine Learning model and generates the required model file.

After training, the project expects:
- `house_model.joblib`
- `house_features.joblib`

---

## ▶️ Running the API

Start the FastAPI server using:

```bash
uvicorn main:app --reload
```

The API will be available at:

```
http://127.0.0.1:8000
```

---

## 📖 API Documentation

FastAPI automatically generates interactive API documentation.

**Swagger UI**
```
http://127.0.0.1:8000/docs
```

**ReDoc**
```
http://127.0.0.1:8000/redoc
```

Swagger UI can be used to test the prediction API directly from the browser.

---

## 🔮 Prediction Workflow

The API receives house-related features from the user.

```
User Input
    ↓
FastAPI Endpoint
    ↓
Input Processing
    ↓
Feature Preparation
    ↓
ML Model
    ↓
Predicted House Price
    ↓
JSON Response
```

---

## 🧪 Example API Request

The exact input fields depend on the features used by the trained model.

A typical request may look like:

```json
{
    "feature_1": 1000,
    "feature_2": 3,
    "feature_3": 2
}
```

The API returns the predicted house price.

> 📌 Use the Swagger documentation at `/docs` to see the exact request schema implemented in the current version of the API.

---

## 📊 Exploratory Data Analysis

The `explore.py` script is used for understanding the dataset before model training.

Typical analysis includes:
- Dataset structure
- Missing values
- Feature distributions
- Data types
- Statistical analysis
- Feature relationships
- Data preprocessing

---

## 🔒 Model File & GitHub

The trained model `house_model.joblib` is approximately 144 MB and is therefore excluded using `.gitignore`.

The `.gitignore` contains:
```
house_model.joblib
```

This prevents the large model file from being accidentally committed to the repository.

> ⚠️ If you clone this repository, make sure the required trained model is available locally before starting the API.

---

## 🔮 Future Improvements

Possible improvements include:
- 📊 Add a web-based frontend
- 📈 Add prediction visualizations
- 🔄 Improve model performance
- 🧠 Experiment with multiple ML algorithms
- 📦 Add automated model training
- 🐳 Dockerize the application
- ☁️ Deploy the API to a cloud platform
- 🗃️ Add database support
- 🔐 Add API authentication
- 📋 Add input validation and error handling
- 📉 Add model performance metrics

---

## 🎯 Learning Objectives

This project demonstrates practical experience with:
- Machine Learning
- Regression-based prediction
- Data preprocessing
- Exploratory Data Analysis
- Model serialization
- REST API development
- FastAPI
- Python backend development
- API documentation
- ML model deployment concepts

---

## 👨‍💻 Author

**Atul Sahu**

GitHub: [https://github.com/atulsahu003](https://github.com/atulsahu003)
