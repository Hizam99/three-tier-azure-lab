# Three-Tier Architecture Lab on Azure (CI/CD with Docker + DevOps Pipelines)

This project demonstrates a full-stack app deployed using a three-tier architecture on Azure.

## 💻 Technologies Used
- Node.js (frontend + backend)
- Azure SQL Database
- Azure DevOps Pipelines (CI/CD)
- Docker & Docker Hub
- Linux VM (self-hosted deployment)
- SonarQube (Code analysis)

## 📦 Structure
- `/frontend` – Frontend app (React or Node UI)
- `/backend` – Backend API with DB connection
- `Dockerfile` – For containerizing both
- `azure-pipelines.yml` – Build + deploy to VM

## 🔁 CI/CD Flow
1. Code pushed to Azure Repos
2. Azure Pipeline builds, tests, analyzes, and pushes Docker image
3. Deploys via SSH to Azure VM

## 🧪 Testing Instructions
- Frontend: `http://<your-vm-ip>:81`
- Backend: `http://<your-vm-ip>:3000`

## ⚠️ Notes
- Resources may be deleted, but this repo shows full structure to recreate.
