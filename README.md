<p align="center">
  <strong> <h1> 🚀 AI-Powered Real-Time Fraud Detection System </h1> <br>End-to-End Machine Learning + Full-Stack Fraud Detection Platform</strong>
</p>

<p align="left">
  <em>Detect anomalous transactions in real time using Machine Learning, FastAPI, PostgreSQL, and React.</em>
</p>

<p align="center">

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge\&logo=fastapi\&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge\&logo=react\&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge\&logo=postgresql\&logoColor=white)
![Scikit Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge\&logo=scikit-learn\&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge\&logo=docker\&logoColor=white)

</p>

<p align="center">

![GitHub Repo Size](https://img.shields.io/github/repo-size/uzumstanley/AI-Powered-Real-Time-Fraud-Detection-System)
![GitHub Last Commit](https://img.shields.io/github/last-commit/uzumstanley/AI-Powered-Real-Time-Fraud-Detection-System)
![GitHub Stars](https://img.shields.io/github/stars/uzumstanley/AI-Powered-Real-Time-Fraud-Detection-System?style=social)

</p>

---

## 🎥 Project Demo

<p align="center">

<a href="https://www.youtube.com/watch?v=YroGtcu9mrM">

<img src="https://img.youtube.com/vi/YroGtcu9mrM/maxresdefault.jpg" alt="AI Fraud Detection System Demo" width="850">

</a>

</p>

<p align="center">
<b>▶️ Click the image above to watch the complete system walkthrough</b>
</p>

---

## 📌 Overview

**AI-Powered Real-Time Fraud Detection System** is an end-to-end machine learning application designed to identify potentially fraudulent or anomalous financial transactions.

The platform combines:

* 🧠 Machine Learning for anomaly detection
* ⚡ FastAPI for high-performance REST APIs
* 🗄️ PostgreSQL for transaction persistence
* ⚛️ React for the monitoring dashboard
* 🧪 Automated testing for reliability
* 🐳 Docker for deployment readiness

The system demonstrates the complete lifecycle of an ML-powered application:

```text
Data
  ↓
Feature Engineering
  ↓
Preprocessing
  ↓
Machine Learning Model
  ↓
Model Serialization
  ↓
FastAPI Backend
  ↓
PostgreSQL Database
  ↓
React Dashboard
  ↓
Real-Time Fraud Monitoring
```

---

# ✨ Key Features

### 🤖 Machine Learning

* Unsupervised **Isolation Forest** anomaly detection
* Transaction and behavioral feature engineering
* Numerical feature scaling
* Categorical feature encoding
* Production-ready preprocessing pipeline
* Model serialization using `joblib`

### ⚡ Backend

* RESTful APIs using **FastAPI**
* Real-time transaction ingestion
* Real-time anomaly/fraud scoring
* PostgreSQL database integration
* Request validation
* Error handling
* CORS configuration
* Swagger/OpenAPI documentation

### ⚛️ Frontend

* Modern React dashboard
* Transaction monitoring
* Fraud/anomaly alerts
* Transaction scoring interface
* API integration using Axios
* React Hooks for state management
* Real-time scoring feedback

### 🧪 Testing & DevOps

* Backend unit tests
* Integration testing
* Environment-based configuration
* Docker-ready architecture
* Deployment-oriented project structure

---

# 🧠 Machine Learning Pipeline

The system uses **Isolation Forest**, an unsupervised machine learning algorithm for detecting unusual transaction patterns.

### Feature Engineering

The model uses transaction-level and user-behavior features including:

| Feature Category     | Examples                      |
| -------------------- | ----------------------------- |
| Transaction          | Amount, duration, type        |
| Account              | Balance, transaction count    |
| User Behavior        | Average transaction amount    |
| Behavioral Deviation | Deviation from user's average |
| Time                 | Transaction hour, day of week |
| Location             | Current and primary location  |
| Channel              | Online, etc.                  |
| Customer             | Age, occupation               |
| Risk Indicators      | Unusual location              |

### Prediction Flow

```text
Raw Transaction
      │
      ▼
Feature Extraction
      │
      ▼
Data Preprocessing
      │
      ├── Numerical Scaling
      │
      └── Categorical Encoding
      │
      ▼
Isolation Forest
      │
      ▼
Anomaly Score
      │
      ▼
Fraud Detection Result
```

---

# 🏗️ System Architecture

```text
                    ┌────────────────────────┐
                    │      React Frontend    │
                    │    Fraud Dashboard     │
                    └────────────┬───────────┘
                                 │
                                 │ HTTP / REST
                                 ▼
                    ┌────────────────────────┐
                    │       FastAPI          │
                    │      Backend API       │
                    └────────────┬───────────┘
                                 │
                    ┌────────────┴────────────┐
                    │                         │
                    ▼                         ▼
          ┌──────────────────┐      ┌──────────────────┐
          │ Machine Learning │      │    PostgreSQL    │
          │ Isolation Forest │      │     Database     │
          └────────┬─────────┘      └──────────────────┘
                   │
                   ▼
          ┌──────────────────┐
          │ Anomaly / Fraud  │
          │     Score        │
          └──────────────────┘
```

---

# 🛠️ Technology Stack

| Layer                | Technology         |
| -------------------- | ------------------ |
| Programming Language | Python, JavaScript |
| Machine Learning     | scikit-learn       |
| ML Algorithm         | Isolation Forest   |
| Data Processing      | Pandas, NumPy      |
| Backend              | FastAPI            |
| API                  | REST               |
| Frontend             | React              |
| HTTP Client          | Axios              |
| Database             | PostgreSQL         |
| Model Serialization  | Joblib             |
| Testing              | Pytest             |
| Containerization     | Docker             |
| Database Management  | pgAdmin            |
| API Documentation    | Swagger / OpenAPI  |
| Version Control      | Git & GitHub       |

---

# 📂 Project Structure

```text
AI-Powered-Real-Time-Fraud-Detection-System/
│
├── app/
│   ├── Database/
│   │   └── schema.sql
│   │
│   ├── model/
│   │   ├── model training scripts
│   │   ├── preprocessing scripts
│   │   └── serialized model files
│   │
│   └── main.py
│
├── frontend/
│   └── React application
│
├── tests/
│   ├── backend tests
│   └── integration tests
│
├── requirements.txt
├── README.md
└── Docker configuration
```

---

# 🚀 Getting Started

## Prerequisites

Make sure the following are installed:

* Python 3.8+
* Node.js
* npm
* PostgreSQL
* Git
* Docker *(optional)*

---

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/uzumstanley/AI-Powered-Real-Time-Fraud-Detection-System.git

cd AI-Powered-Real-Time-Fraud-Detection-System
```

---

## 2️⃣ Configure PostgreSQL

Create a PostgreSQL database:

```text
frauddb
```

Then execute the database schema:

```bash
psql -U <username> -d frauddb -f app/Database/schema.sql
```

---

## 3️⃣ Configure Environment Variables

Create a `.env` file inside the backend application.

```env
DATABASE_URL=postgresql://<username>:<password>@localhost:5432/frauddb
JWT_SECRET=your_secret_key
```

> ⚠️ **Security:** Never commit real passwords, API keys, tokens, or secrets to GitHub.

---

## 4️⃣ Install Backend Dependencies

```bash
cd app

pip install -r ../requirements.txt
```

---

## 5️⃣ Start the Backend

```bash
uvicorn main:app --reload
```

The API will be available at:

```text
http://127.0.0.1:8000
```

### Interactive API Documentation

FastAPI automatically provides Swagger documentation:

```text
http://127.0.0.1:8000/docs
```

---

## 6️⃣ Start the Frontend

Open a new terminal:

```bash
cd frontend

npm install

npm start
```

The React application will run at:

```text
http://localhost:3000
```

---

# 📡 API Usage

## Score a Transaction

### Endpoint

```http
POST /transactions/score
```

### Sample Request

```json
{
  "account_id": "test_account_123",
  "TransactionAmount": 420.50,
  "CustomerAge": 35,
  "TransactionDuration": 6.2,
  "LoginAttempts": 1,
  "AccountBalance": 15000.0,
  "user_transaction_count": 8,
  "user_avg_transaction_amount": 400.0,
  "deviation_from_user_avg": 20.5,
  "transaction_hour": 10,
  "transaction_day_of_week": 1,
  "TransactionType": "Debit",
  "Location": "Chicago",
  "Channel": "Online",
  "CustomerOccupation": "Analyst",
  "user_primary_location": "Chicago",
  "is_unusual_location": "False"
}
```

The transaction is processed through the feature engineering and preprocessing pipeline before being evaluated by the Isolation Forest model.

---

# 📊 Dashboard Capabilities

The React dashboard is designed to provide an operational view of the fraud detection system.

### Transaction Monitoring

View transaction information and scoring results through the dashboard.

### Fraud Alerts

Identify transactions flagged as anomalous by the machine learning model.

### Transaction Scoring

Submit transaction information and receive an immediate prediction.

### API Integration

The frontend communicates with the FastAPI backend through REST APIs using Axios.

---

# 🧪 Testing

Run the backend test suite:

```bash
pytest
```

For a specific test file:

```bash
pytest tests/test_main.py
```

Frontend tests can be executed with:

```bash
npm test
```

---

# 🔐 Engineering & Security Practices

The project follows development practices intended for production-oriented applications:

* Environment variables for configuration
* No hard-coded credentials
* RESTful API architecture
* Input validation
* Error handling
* CORS configuration
* Separation of frontend/backend/ML/database layers
* Automated testing
* Reusable ML preprocessing
* API documentation
* Docker-ready deployment

---

# 💼 Skills Demonstrated

This project demonstrates practical experience across multiple engineering areas.

### Software Engineering

* REST API Development
* Backend Architecture
* Database Design
* API Integration
* Error Handling
* Automated Testing

### Machine Learning

* Unsupervised Learning
* Anomaly Detection
* Isolation Forest
* Feature Engineering
* Data Preprocessing
* Model Serialization
* ML Inference

### Full-Stack Development

* React
* FastAPI
* PostgreSQL
* Axios
* REST APIs
* End-to-End Application Architecture

### DevOps

* Docker
* Environment Configuration
* Testing
* Deployment-Oriented Development

---

# 📈 Future Improvements

The project can be extended with:

* [ ] JWT Authentication
* [ ] Role-Based Access Control
* [ ] Redis caching
* [ ] Real-time event streaming
* [ ] Model performance monitoring
* [ ] Automated model retraining
* [ ] SHAP-based explainability
* [ ] Advanced fraud analytics
* [ ] Docker Compose
* [ ] GitHub Actions CI/CD
* [ ] Cloud deployment
* [ ] Centralized logging and monitoring

---

# 🗺️ Project Roadmap

View the development roadmap:

👉 **[GitHub Project Roadmap](https://github.com/users/uzumstanley/projects/2/views/1)**

---

# 🎥 Watch the Full Demo

<p align="center">

<a href="https://www.youtube.com/watch?v=YroGtcu9mrM">

<img src="https://img.youtube.com/vi/YroGtcu9mrM/maxresdefault.jpg" alt="Watch Fraud Detection System Demo" width="800">

</a>

</p>

<p align="center">

<strong>▶️ Watch the complete project demonstration on YouTube</strong>

</p>

---

# 🌟 Why This Project?

This project was built to demonstrate how a machine learning model can be integrated into a complete software product rather than remaining as an isolated notebook or model.

It connects:

**Machine Learning → Backend Engineering → Database → Frontend → Testing → Deployment**

This makes the project relevant to roles such as:

* Software Engineer
* Backend Developer
* Full-Stack Developer
* Machine Learning Engineer
* AI Engineer
* Data Engineer

---

# 👩‍💻 Author

**Uz umstanley**

AI/ML • Full-Stack Development • Backend Engineering • Data Engineering

---

## ⭐ Support

If you find this project useful or interesting, consider giving it a ⭐ on GitHub.

<p align="center">

<b>Built with Python • FastAPI • React • PostgreSQL • Machine Learning</b>

</p>


## 🙋‍♂️ Contact

For questions or collaboration, open an issue or contact [uzumstanley](https://github.com/uzumstanley).

