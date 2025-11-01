🏥 Healthcare Microservices Demo

By Areeba Asif
A containerized microservices-based healthcare system built with Flask, Docker, Kubernetes, and GitHub Actions.
This project demonstrates a complete CI/CD workflow — from code to containerization and deployment — using modern DevOps tools.

🧠 Overview

The system consists of three main services:

🧑‍⚕️ Doctors Service – Provides a list of available doctors.

📅 Appointments Service – Manages patient appointments.

💻 Frontend Service – Displays doctors and appointments in a simple UI.

All services are containerized and deployed using Docker Compose and Kubernetes (K8s), with GitHub Actions automating image builds and updates.

⚙️ Key Features

Microservices Architecture — Independent Flask apps for each component

CI/CD Pipelines — Automated Docker builds via GitHub Actions

Kubernetes Deployment — ConfigMaps, Secrets, Deployments, and Services for each module

Docker Compose — Local multi-container setup for quick testing

MongoDB Integration — For persistent data storage

🧰 Technologies Used

Python (Flask, REST APIs)

Docker & Docker Compose

Kubernetes (YAML Configs)

GitHub Actions (CI/CD)

MongoDB

HTML / JS Frontend

🧩 Project Structure
├── appointments/
│   ├── app.py
│   ├── Dockerfile
│   ├── k8s/
│   │   └── app.yaml
│
├── doctors/
│   ├── app.py
│   ├── Dockerfile
│   ├── k8s/
│   │   └── app.yaml
│
├── frontend/
│   ├── index.html
│   ├── main.js
│   ├── Dockerfile
│   ├── k8s/
│   │   └── app.yaml
│
├── .github/workflows/
│   ├── appointments-cicd.yml
│   ├── doctors-cicd.yml
│   └── frontend.yml
│
├── docker-compose.yml
└── k8s/
    ├── app.yaml
    ├── doctors-configmap.yaml
    └── mongo-secret.yaml

🚀 CI/CD Workflow

Each service has its own GitHub Actions pipeline:

Automatically builds a Docker image when code changes are pushed.

Tags the image with the commit hash.

Updates the docker-compose.yml file with the new version.

Commits and pushes the update back to the main branch.

🧾 Learning Outcomes

Implementing microservices using Flask

Setting up automated CI/CD pipelines with GitHub Actions

Using Docker Compose for local orchestration

Managing Kubernetes deployments with Secrets and ConfigMaps

Understanding DevOps workflows end-to-end

🏫 Academic Context

This project was created as part of a DevOps / MLOps course assignment to demonstrate full-stack deployment automation.
