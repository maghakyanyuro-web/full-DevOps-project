# 🚀 full-DevOps-project

A production-style DevOps project demonstrating containerization, 
cloud deployment, and CI/CD automation.

## 🛠️ Tech Stack

- **Node.js** — Backend application
- **Docker** — Containerization
- **AWS EC2** — Cloud deployment
- **GitHub Actions** — CI/CD pipeline
- **Linux (Ubuntu)** — Server environment

## 📦 Project Structure

full-DevOps-project/
├── app/
│   ├── index.js
│   ├── Dockerfile
│   ├── package.json
│   └── .dockerignore
└── .github/
    └── workflows/
        └── ci-cd.yml

## 🔄 CI/CD Pipeline

Every push to `main` branch automatically:
1. Connects to AWS EC2 via SSH
2. Pulls latest code
3. Builds Docker image
4. Restarts container with new version

## 🚀 Run Locally
```bash
docker build -t full-devops-project ./app
docker run -p 3000:3000 full-devops-project
```

Open http://localhost:3000

## ☁️ Deployment

Deployed on AWS EC2 (Ubuntu 22.04, t3.micro)

## 📌 Coming Soon

- Terraform (Infrastructure as Code)
- Kubernetes deployment
