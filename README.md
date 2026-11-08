# 🌤️ Historical Weather Data REST API (Python & Flask)

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-2.x-black?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Pandas](https://img.shields.io/badge/Pandas-Data-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)

A lightweight, high-performance RESTful API microservice built with **Flask** and **Pandas** that processes historical meteorological records and serves structured JSON endpoints with multi-parameter filtering.

---

## 🚀 API Endpoints Specification

| Method | Endpoint | Description | Output Format |
|:---:|:---|:---|:---:|
| `GET` | `/` | Web UI displaying registered stations directory | HTML |
| `GET` | `/api/v1/<station>/<date>` | Query specific station temperature by date (`YYYYMMDD`) | JSON |
| `GET` | `/api/v1/<station>` | Fetch complete historical time-series for a station | JSON Array |
| `GET` | `/api/v1/yearly/<station>/<year>` | Fetch filtered records by year (`YYYY`) | JSON Array |

---

## ⚡ Quickstart

### 1. Clone & Install Dependencies
```bash
git clone https://github.com/nabilmushfique460/Build-a-Weather-Data-API.git
cd Build-a-Weather-Data-API
pip install -r requirements.txt
```

### 2. Run the API Server
```bash
python main.py
```
The server will boot locally at `http://127.0.0.1:5000/`.

---

## 📝 Example JSON Response

`GET /api/v1/10/19881025`
```json
{
  "station": "10",
  "date": "19881025",
  "temperature": 11.2
}
```

---

## 💼 Custom API Development Services
Need custom Python REST APIs, FastAPI/Flask microservices, or database integration for your product?

- **Developer:** S.M. Nabil Mushfique
- **Email:** [nabilmushfique460@gmail.com](mailto:nabilmushfique460@gmail.com)
- **Services:** Custom Flask/FastAPI REST APIs, Data Transformation, Database Integrations (SQLite/MySQL/PostgreSQL).
