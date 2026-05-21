# Digital Epidemiology System for Real-Time Disease Surveillance

![alt text](outputs/chart2.jpg)

## Overview

The Digital Epidemiology System for Real-Time Disease Surveillance is an AI-powered public health monitoring platform designed to track, analyze, visualize, and predict disease outbreaks in real time.

The system integrates machine learning, geospatial analysis, real-time monitoring, and epidemiological analytics to support early outbreak detection and informed public health decision-making.

This project demonstrates the practical application of:
- Data Science
- Machine Learning
- Epidemiology
- GIS & Spatial Analytics
- Real-Time Surveillance Systems
- API Development
- Health Informatics

---

# Features

## Real-Time Disease Surveillance
- Monitor disease cases continuously
- Track outbreak hotspots dynamically
- Analyze disease spread patterns

## Machine Learning Disease Prediction
- Predict likely disease categories
- Risk-based outbreak analysis
- Automated classification using Random Forest

## Interactive GIS Dashboard
- Geospatial visualization of disease cases
- Heatmaps and outbreak mapping
- Real-time disease distribution analysis

## Outbreak Detection System
- Automatically detects abnormal case spikes
- Generates outbreak alerts by region and disease type

## REST API Backend
- FastAPI-powered API endpoints
- Real-time prediction services
- Statistical reporting endpoints

## Epidemiological Analytics
- Daily trend analysis
- Severity monitoring
- Recovery and mortality tracking

---

# Project Architecture

```text
                ┌────────────────────┐
                │  Synthetic Dataset │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ Data Preprocessing │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ Machine Learning   │
                │ Random Forest      │
                └─────────┬──────────┘
                          │
          ┌───────────────┴───────────────┐
          ▼                               ▼
┌───────────────────┐          ┌──────────────────┐
│ Real-Time API     │          │ GIS Dashboard    │
│ FastAPI Backend   │          │ Plotly Maps      │
└───────────────────┘          └──────────────────┘
          │                               │
          ▼                               ▼
┌───────────────────┐          ┌──────────────────┐
│ Outbreak Alerts   │          │ Epidemiological  │
│ Notification Sys  │          │ Trend Analytics  │
└───────────────────┘          └──────────────────┘
Technologies Used
Programming Language
Python
Backend Framework
FastAPI
Machine Learning
Scikit-learn
Random Forest Classifier
Data Processing
Pandas
NumPy
Visualization
Plotly
Mapbox
API Server
Uvicorn
Geospatial Analytics
Latitude & Longitude Mapping
Spatial Disease Visualization
Dataset Information

### The project uses a synthetic epidemiological dataset containing:

Disease Cases
Patient Demographics
Geographic Coordinates
Environmental Conditions
Severity Levels
Risk Scores
Recovery Status
Diseases Included
Malaria
Cholera
COVID-19
Lassa Fever
Dengue
Typhoid
Ebola
Installation
Clone Repository
git clone https://github.com/yourusername/Digital-Epidemiology-System-for-Real-Time-Disease-Surveillance.git
Navigate into Project Folder
cd Digital-Epidemiology-System-for-Real-Time-Disease-Surveillance
Install Dependencies
pip install -r requirements.txt
Required Libraries
fastapi
uvicorn
pandas
numpy
scikit-learn
plotly
pydantic
Run the Project
Start the FastAPI Server
python app.py

Server runs at:

http://127.0.0.1:8000
API Endpoints
Home Endpoint
GET /

Returns system status.

Disease Prediction
POST /predict
Sample Request
{
  "patient_age": 34,
  "temperature_celsius": 39.2,
  "humidity_percent": 80,
  "risk_score": 0.87,
  "state": "Lagos",
  "gender": "Male",
  "severity_level": "Severe"
}
Sample Response
{
  "predicted_disease": "Malaria",
  "timestamp": "2026-05-21 14:20:01"
}
Outbreak Alerts
GET /alerts

Returns regions with unusually high disease cases.

Disease Statistics
GET /statistics

Returns total disease counts.

Machine Learning Workflow
Data Preprocessing
Label Encoding
Feature Engineering
Data Cleaning
Model Training
Random Forest Classifier
Train/Test Split
Supervised Learning
Evaluation
Classification Report
Accuracy Metrics
Disease Prediction Analysis
Visualization Features
GIS Disease Map
Interactive outbreak visualization
Real-time spatial disease tracking
Epidemiological Trend Charts
Daily case trends
Temporal outbreak analysis
Real-World Applications

### This system can support:

Ministries of Health
Hospitals
WHO Surveillance Programs
NGOs
Epidemic Monitoring Agencies
Public Health Researchers

### Potential applications include:

Cholera outbreak monitoring
Malaria hotspot detection
Pandemic surveillance
Early warning systems
Health emergency response
Future Improvements
Deep Learning Disease Forecasting
IoT Health Sensor Integration
Mobile Application
SMS Alert System
Cloud Deployment
Real-Time Streaming with Kafka
Advanced GIS Heatmaps
AI-Based Mortality Prediction
Integration with Public Health APIs
Sample Dashboard Concepts
Disease Heatmaps
Regional disease concentration analysis
Risk Prediction
AI-generated outbreak risk scoring
Time-Series Analytics
Temporal spread visualization
Folder Structure
Digital-Epidemiology-System/
│
├── app.py
├── requirements.txt
├── README.md
├── digital_epidemiology_synthetic_dataset.csv
│
├── models/
│   └── trained_model.pkl
│
├── notebooks/
│   └── disease_analysis.ipynb
│
├── dashboards/
│   └── surveillance_dashboard.py
│
└── assets/
    └── images/


## Author
     Jonah Buka

Data Scientist | Machine Learning Engineer | Geospatial & Environmental Analytics Researcher

License

This project is licensed under the MIT License.

Acknowledgements

Special thanks to:

Open-source Python community
Public health researchers
Epidemiology and GIS communities
Machine learning contributors
Project Goals

The primary objective of this project is to demonstrate how artificial intelligence, geospatial intelligence, and real-time analytics can improve disease surveillance, outbreak detection, and public health response systems globally.
