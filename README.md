# 🚀 Deploy a Containerized Flask Web App on AWS ECS with CI/CD

## 📌 Project Overview

This project demonstrates how to deploy a containerized Flask web application on **Amazon ECS Fargate** using **Docker**, **Amazon ECR**, and **GitHub Actions** for Continuous Integration and Continuous Deployment (CI/CD).

Whenever code is pushed to the `main` branch, GitHub Actions automatically builds the Docker image, pushes it to Amazon ECR, and deploys the latest version to Amazon ECS.

---

## 🛠️ Technologies Used

- Python (Flask)
- Docker
- Amazon ECR
- Amazon ECS (Fargate)
- Application Load Balancer (ALB)
- GitHub Actions
- AWS IAM
- Amazon CloudWatch
- Git & GitHub

---

## 📂 Project Structure

```
ecs-cicd-project/
│
├── app.py
├── Dockerfile
├── requirements.txt
└── .github/
    └── workflows/
        └── deploy.yml
```

---

## ⚙️ Architecture

```
Developer
    │
    ▼
GitHub Repository
    │
    ▼
GitHub Actions
(Build Docker Image)
    │
    ▼
Amazon ECR
(Store Docker Image)
    │
    ▼
Amazon ECS Fargate
(Run Container)
    │
    ▼
Application Load Balancer
    │
    ▼
Users
```

---

## 🚀 Features

- Containerized Flask application using Docker
- Docker image stored in Amazon ECR
- Deployed using Amazon ECS Fargate
- Application exposed through Application Load Balancer
- Automated deployment with GitHub Actions
- Cloud-native deployment on AWS

---

## 📋 Prerequisites

- AWS Account
- Docker Desktop
- AWS CLI
- Git
- GitHub Account

---

## ▶️ Run Locally

Clone the repository:

```bash
git clone https://github.com/Santhipriya7/ecs-cicd-project.git
```

Move into the project directory:

```bash
cd ecs-cicd-project
```

Build the Docker image:

```bash
docker build -t flask-app .
```

Run the container:

```bash
docker run -p 5000:5000 flask-app
```

Open your browser:

```
http://localhost:5000
```

---

## ☁️ Deployment Steps

1. Build Docker Image
2. Push Docker Image to Amazon ECR
3. Create ECS Cluster
4. Create Task Definition
5. Create ECS Service
6. Configure Application Load Balancer
7. Configure GitHub Actions CI/CD
8. Push Code to GitHub
9. Automatic Deployment to ECS

---

## 🔐 GitHub Secrets

The following GitHub Secrets are used:

- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- AWS_REGION
- ECS_CLUSTER
- ECS_SERVICE
- ECR_REPOSITORY

---

## 📸 Project Screenshots

Add screenshots here:

- ECS Cluster
- ECS Service
- Amazon ECR Repository
- GitHub Actions Workflow
- Running Application

---

## 👩‍💻 Author

**Santhipriya**

- GitHub: https://github.com/Santhipriya7

---

## ⭐ Learning Outcomes

Through this project I learned:

- Docker containerization
- Amazon ECR
- Amazon ECS Fargate
- Application Load Balancer
- GitHub Actions CI/CD
- AWS IAM
- Continuous Deployment
- Cloud Application Deployment

---
