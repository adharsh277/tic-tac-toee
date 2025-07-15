# ♟️ Tic-Tac-Toe Web App: CI/CD + AKS Deployment

![Azure](https://img.shields.io/badge/Azure-Kubernetes-blue?logo=azure-kubernetes-service)
![Docker](https://img.shields.io/badge/Docker-Containerized-green?logo=docker)
![GitHub Actions](https://img.shields.io/badge/CI/CD-Automation-orange?logo=githubactions)
![Status](https://img.shields.io/badge/Status-Deployed-brightgreen)

## 📌 Project Overview

This project demonstrates a **complete DevOps lifecycle** for a Python-based Tic-Tac-Toe game:

- 🐍 Python Web App (`Flask`)
- 🐳 Dockerized for containerization
- 🔁 GitHub Actions for CI/CD
- ☸️ Deployed to **Azure Kubernetes Service (AKS)**
- 🌐 Accessed via a LoadBalancer service

---

## 🚀 Features

- ✅ Modern DevOps Workflow with CI/CD
- ✅ Docker image build & push using GitHub Actions
- ✅ AKS deployment with auto-triggered GitHub Action
- ✅ Scalable microservice architecture
- ✅ Clean folder structure with YAML, Docker, and app files


## 🧱 Tech Stack

| Layer              | Tools / Services                      |
|--------------------|----------------------------------------|
| Language           | Python 3.10                            |
| Web Framework      | Flask                                  |
| Containerization   | Docker                                 |
| CI/CD Pipeline     | GitHub Actions                         |
| Kubernetes Cluster | Azure Kubernetes Service (AKS)         |
| Hosting            | Azure Cloud                            |



## ⚙️ CI/CD Workflow

### 🔨 Build & Push Docker Image

- Runs on every push to `main`
- Builds Docker image
- Pushes to Docker Hub using `DOCKER_USERNAME` secret

### 🚀 Deploy to AKS

- Runs automatically after image build
- Uses `KUBE_CONFIG_DATA` secret to connect to AKS
- Applies all YAMLs in the `k8s/` folder

---
 ## Service exposes the app on an external IP:

cpp
Copy
Edit
http://4.255.100.81/

## 🔐 Secrets Used

| Secret Name          | Description                                    |
|----------------------|------------------------------------------------|
| `DOCKER_USERNAME`    | Your Docker Hub username                      |
| `DOCKER_PASSWORD`    | Docker Hub password or access token            |
| `KUBE_CONFIG_DATA`   | Base64-encoded `~/.kube/config` from AKS       |

---

## ✅ Deployment Access

Once deployed:

`bash
kubectl get services

---



🧠 Learning Outcome
Full DevOps workflow using GitHub Actions

Working with AKS clusters and service exposure

Dockerizing Python GUI/Web apps

Real-time CI/CD pipelines with secret handling

🙌 Acknowledgements
Original project by aqeelanwar

DevOps setup & deployment customized and executed by adharsh277 ✨

## 📣 Contact

📧 [Adharsh](https://www.linkedin.com/in/adharsh277/) – LinkedIn  
🌍 [Adharsh](https://github.com/adharsh277) – GitHub



