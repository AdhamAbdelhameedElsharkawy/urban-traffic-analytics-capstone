# Metropolitan City Traffic Analysis - Capstone Project

This project is the final capstone for the German University in Cairo's Data Engineering & AI Diploma. It provides a comprehensive end-to-end data pipeline for analyzing urban traffic patterns using real New York City traffic datasets.

## 🚦 Project Overview

We analyze traffic trends in a large metropolitan city using public NYC Taxi datasets (Bus, Subway, Taxi). The pipeline performs:

- Ingestion of large-scale raw data
- Preprocessing & cleaning
- Data warehousing
- Exploratory data analysis (EDA)
- Machine Learning for ride duration prediction
- Dashboarding using Apache Superset

## 🏗️ Architecture

This project leverages a modern data engineering stack:

- **Apache Airflow** – DAG orchestration
- **PostgreSQL** – Data warehouse
- **Docker** – Containerized deployment
- **Pandas, Scikit-learn** – Data processing & ML
- **Apache Superset** – Visualization & BI
- **Jupyter Notebooks** – EDA & experimentation

## 📂 Project Structure

```
├── Infra/                  # Docker setup and infra structure
├── Bus_BusLanes/              # Code for Bus and bus lanes datasets
├── Subway/                  # Code for Subway dataset
├── Taxi/                  # Code for Taxi dataset
├── ML-Model/              # Machine learning Model code for fare predication
├── Sample data/              # Data samples to be used with Airflow pipeline dags
├── Capstone Project-NYC Transportation Analysis.pptx              # Small presentation for the project and some analytics
└── README.md
```

## 🛠️ How to Run

1. Clone the repository
2. Ensure Docker is installed
3. From Docker folder Run (add build as bash parameter to rebuild containers):

```bash init.sh build `` to start up postgress and Airflow
```bash init_super_set `` to start up superset


```

4. Access Airflow at: `http://localhost:8080`
5. Access Superset at: `http://localhost:8088`

## 🧠 Machine Learning

We trained models on Taxi data to predict trip fare using:
- Deep Learning FFNN Model

## 📊 Dashboards

Superset dashboards provide key insights:
- Trip durations over time
- Day vs. night ride trends

## 👥 Authors

- **Abdullah Kamal** - Senior Data Steward - Schneider Electric
- **Ahmed Abdullah** - 	
- **Adham Abdelhameed ElSharkawy** – Cloud Solution Architect - Microsoft
- **Ajeeb ElAmeen** - 
- **Osama ElNaggar** - Data Management Lead - Dana Petroleum

## 📜 License

MIT License

## 🌐 Public Datasets Used

- [NYC Traffic Commission Data](https://www.nyc.gov/html/dot/html/about/datafeeds)(https://catalog.data.gov/dataset/mta-subway-stations)(https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

---

> This project aims to serve as a reusable and extendable framework for urban mobility and traffic analysis. Contributions welcome!
