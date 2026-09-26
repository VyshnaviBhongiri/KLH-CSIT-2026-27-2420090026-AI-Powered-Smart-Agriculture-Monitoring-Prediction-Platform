# 🌱 AI-Smart-Agriculture

## AI-Powered Smart Agriculture Monitoring and Crop Disease Prediction Platform

---

# Team Members

| **Name**          | **Student ID** |
| ----------------- | -------------- |
| B. Vaishnavi      | 2420090026     |
| S. Lahari Krishna | 2420090055     |

---

# Supervisor

**Supervisor Name:** Ms. G. Lavanya

**Department:** CSE

**Academic Year:** 2026–2027

---

# Abstract

Agriculture plays an important role in food production, but farmers face several challenges in monitoring crop health, detecting diseases at an early stage, and managing environmental conditions. Manual crop inspection is time-consuming, while changing temperature, humidity, and soil-moisture conditions can affect crop growth.

This project proposes an **AI-Powered Smart Agriculture Monitoring and Crop Disease Prediction Platform** that integrates artificial intelligence, environmental monitoring, and intelligent recommendations into a centralized web application.

The system uses crop leaf images for disease prediction and environmental parameters such as temperature, humidity, and soil moisture for crop-health analysis. Based on the prediction and environmental conditions, the system provides recommendations related to irrigation, fertilizer usage, disease management, and preventive measures.

The platform is developed using **React, FastAPI, PostgreSQL, Python, Deep Learning, Docker, MLflow, GitHub Actions, and AWS**. The proposed system aims to support data-driven crop monitoring and provide farmers with timely and useful crop-health insights.

---

# Project Objectives

* Detect crop diseases using AI/Deep Learning.
* Monitor temperature, humidity, and soil moisture.
* Provide intelligent irrigation recommendations.
* Provide fertilizer recommendations.
* Provide disease-management suggestions.
* Analyze crop health using image and environmental data.
* Provide an interactive farmer dashboard.
* Maintain historical disease predictions and reports.
* Build a scalable and continuously improvable platform.

---

# User Roles

## Farmer / User

* Register and log in.
* Upload crop/leaf images.
* Enter or receive environmental data.
* View disease predictions.
* View crop-health status.
* Receive irrigation recommendations.
* Receive fertilizer recommendations.
* View disease-management suggestions.
* View prediction history.
* Monitor environmental conditions.

## Administrator

* Manage registered users.
* Manage crop and disease information.
* Manage datasets.
* Monitor prediction activity.
* View system statistics.
* Maintain disease information.
* Monitor platform activity.

---

# AI Integration

## AI Objective

Predict crop diseases from leaf images and support crop-health analysis using environmental information.

## Input Features

### Image Features

* Crop/leaf image
* Image characteristics extracted by the deep-learning model

### Environmental Features

* Temperature
* Humidity
* Soil moisture

## Output

The system provides:

* Healthy / Diseased classification
* Disease type
* Prediction confidence
* Crop-health status
* Irrigation recommendation
* Fertilizer recommendation
* Disease-management recommendation

## AI Workflow

```text
Crop Leaf Image
       ↓
Image Preprocessing
       ↓
Deep Learning Model
       ↓
Disease Prediction
       ↓
Confidence Score
       ↓
Crop Health Analysis
       ↓
Recommendation Engine
       ↓
Irrigation / Fertilizer /
Disease Management
```

---

# Technology Stack

| **Component**        | **Technology**     |
| -------------------- | ------------------ |
| Frontend             | React.js           |
| Build Tool           | Vite               |
| Backend              | FastAPI            |
| Programming Language | Python             |
| Database             | PostgreSQL         |
| AI/ML                | Deep Learning      |
| ML Lifecycle         | MLflow             |
| Repository           | GitHub             |
| CI/CD                | GitHub Actions     |
| Containerization     | Docker             |
| Cloud                | AWS                |
| Project Management   | Jira / Trello      |

---

# Mandatory Folder Structure

```text
AI-Smart-Agriculture/
│
├── README.md
│
├── src/
│   ├── frontend/
│   ├── backend/
│   ├── ai-service/
│   └── database/
│
├── docs/
│   ├── requirements/
│   ├── architecture/
│   ├── user-stories/
│   └── sprint-documents/
│
├── data/
│   ├── datasets/
│   └── dataset-references.md
│
├── results/
│   ├── model-results/
│   ├── screenshots/
│   └── evaluation-results/
│
└── reports/
    ├── sprint-reports/
    ├── progress-reports/
    └── final-report/
```

This follows the same kind of mandatory project organization shown in the sample README you provided.

---

# Setup Instructions

## Prerequisites

* Python 3.10+
* Node.js
* PostgreSQL
* Git
* VS Code
* Docker (Optional)
* AWS Account (for deployment)
* MLflow

---

# Planned Setup Process

1. Clone the repository.
2. Configure PostgreSQL database.
3. Configure FastAPI backend.
4. Install React dependencies.
5. Configure AI/ML service.
6. Configure the disease dataset.
7. Train the disease prediction model.
8. Connect frontend with backend APIs.
9. Start the application.
10. Test the complete workflow.

---

# Execution Instructions

## Backend

```bash
cd src/backend
python -m venv .venv
```

### Windows

```bash
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run FastAPI:

```bash
uvicorn app.main:app --reload
```

Backend:

```text
http://127.0.0.1:8000
```

Swagger:

```text
http://127.0.0.1:8000/docs
```

---

# Frontend

```bash
cd src/frontend
npm install
npm run dev
```

Frontend:

```text
http://localhost:5173
```

---

# AI Service

```bash
cd src/ai-service
pip install -r requirements.txt
python train.py
```

The trained model will be used for crop disease prediction.

---

# Database

PostgreSQL database:

```text
Database Name: smart_agriculture
Port: 5432
```

Example:

```sql
CREATE DATABASE smart_agriculture;
```

---

# Agile Development Approach

The project follows the **Scrum Framework**.

## Scrum Activities

* Product Backlog
* Sprint Planning
* Sprint Development
* Daily Scrum
* Sprint Review
* Sprint Retrospective

## Agile Tool

**Jira / Trello** can be used for:

* User Stories
* Task Management
* Sprint Planning
* Backlog Management
* Progress Tracking
* Issue Tracking

---

# Current Phase Status

## Phase

**Requirements Analysis and System Design**

## Completed

* Project title finalized.
* Problem statement identified.
* Project objectives defined.
* Technology stack selected.
* System workflow designed.
* Major modules identified.
* AI integration approach defined.
* Initial project architecture prepared.
* UI design/prototype prepared.

## In Progress

* React frontend development.
* FastAPI backend development.
* PostgreSQL database setup.
* Dataset preparation.
* AI model development.
* API integration.

## Not Yet Started

* Complete model training.
* Real-time IoT sensor integration.
* AWS deployment.
* GitHub Actions CI/CD.
* MLflow production integration.
* Complete system testing.
* Security testing.

> Update these statuses as the actual implementation progresses.

---

# Dataset Information

The project will use publicly available crop-disease datasets for machine-learning model development and evaluation.

Potential dataset sources include:

* PlantVillage Dataset
* Kaggle crop-disease datasets
* Other publicly available agricultural image datasets

The dataset will contain crop/leaf images organized according to disease classes.

Example:

```text
dataset/
│
├── Healthy/
├── Early_Blight/
├── Late_Blight/
└── Leaf_Spot/
```

The exact dataset and class distribution will be documented after dataset selection.

---

# Evaluation Metrics

## AI Model Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

## System Metrics

* Response Time
* Prediction Time
* Reliability
* Usability
* Recommendation Response
* Dashboard Performance

---

# Expected Outcomes

* Automated crop disease detection.
* Early identification of crop-health problems.
* Environmental condition monitoring.
* Intelligent irrigation recommendations.
* Fertilizer recommendations.
* Disease-management guidance.
* Centralized crop-health dashboard.
* Historical prediction records.
* Scalable agriculture monitoring platform.

---

# Future Scope

* Real-time IoT sensor integration.
* Automatic soil-moisture monitoring.
* Automated irrigation control.
* Support for additional crops.
* Support for additional diseases.
* Improved deep-learning models.
* Weather API integration.
* Mobile application.
* AWS cloud deployment.
* Automated CI/CD pipelines.
* Continuous ML model monitoring.
* Automated model retraining.
* Multilingual farmer support.

---

# Project Status Summary

**Current Status:** Requirements Analysis & System Design

**Implementation Status:** Development in Progress

**AI Model Status:** Dataset / Model Development

**Frontend Status:** Development in Progress

**Backend Status:** Development in Progress

**Database Status:** Development in Progress

**Testing Status:** Not Yet Started

**Deployment Status:** Planned

---

# Project Workflow

```text
                Farmer
                   │
                   ▼
          React Web Application
                   │
        ┌──────────┴──────────┐
        ▼                     ▼
   Leaf Image            Environment
        │                Data
        ▼                     │
  Image Processing             │
        │                     │
        └──────────┬──────────┘
                   ▼
            AI/ML Prediction
                   │
                   ▼
           Crop Health Analysis
                   │
                   ▼
          Recommendation Engine
                   │
        ┌──────────┼──────────┐
        ▼          ▼          ▼
    Irrigation  Fertilizer  Disease
                           Management
                   │
                   ▼
              Dashboard
                   │
                   ▼
             PostgreSQL
```

---

# Team

### B. Vaishnavi

**Student ID:** 2420090026

### S. Lahari Krishna

**Student ID:** 2420090055

### Guide

**Ms. G. Lavanya**

### Department

**CSE**

### Academic Year

**2026–2027**
