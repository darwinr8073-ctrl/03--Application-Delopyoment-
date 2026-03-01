📄 README.md
# 🚀 DevOps CI/CD Pipeline Project (React App Deployment)

## 📌 Project Overview
This project demonstrates a complete **DevOps CI/CD pipeline** using GitHub, Jenkins, Docker, and AWS EC2.  
A React application is containerized using Docker and automatically built, pushed, and deployed based on Git branch workflows.

The pipeline implements modern DevOps practices including:
- Continuous Integration
- Continuous Deployment
- Containerization
- Cloud Deployment
- Application Monitoring

---

## 🏗️ Architecture

Developer → GitHub → Jenkins → Docker Build → Docker Hub → AWS EC2 → Running Container → Monitoring

### Branch Strategy
- **dev branch** → Build & push development Docker image
- **main branch** → Build production image & auto-deploy application

---

## 🛠️ Technologies Used

- **Frontend**: React.js
- **CI/CD**: Jenkins
- **Containerization**: Docker & Docker Compose
- **Cloud Platform**: AWS EC2 (Amazon Linux)
- **Version Control**: Git & GitHub
- **Web Server**: Nginx
- **Monitoring**: Uptime Kuma
- **Scripting**: Bash

---

## ⚙️ Project Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/<your-username>/devops_build.git
cd devops_build
2️⃣ Run Locally
npm install
npm start

Application runs on:

http://localhost:3000
🐳 Docker Setup
Build Image
docker build -t react-app .
Run Container
docker run -d -p 80:80 react-app

Application runs on:

http://localhost
📦 Docker Compose
docker-compose up --build -d
🔄 CI/CD Pipeline (Jenkins)
Jenkins Workflow

Developer pushes code to dev branch

Jenkins builds Docker image

Image pushed to Docker Hub (dev repository)

Pull request merged into main

Jenkins builds production image

Container automatically deployed on AWS EC2

🧾 Jenkins Build Logic
docker build -t react-app .

if branch == dev:
   push dev image

if branch == main:
   push prod image
   deploy container
☁️ AWS Deployment

EC2 Instance: Amazon Linux 2

Ports Open:

22 → SSH

80 → Application Access

8080 → Jenkins

3001 → Monitoring

Application URL:

http://<EC2-PUBLIC-IP>
📊 Monitoring

Monitoring implemented using Uptime Kuma.

Features:

HTTP health checks

Status monitoring

Downtime alerts

Open-source monitoring dashboard

Access:

http://<EC2-IP>:3001
📁 Project Structure
devops_build/
│
├── Dockerfile
├── docker-compose.yml
├── build.sh
├── deploy.sh
├── src/
├── public/
└── README.md
✅ Features Implemented

✔ Multi-stage Docker build
✔ Branch-based CI/CD pipeline
✔ Automated deployment
✔ Docker Hub integration
✔ AWS cloud hosting
✔ Health monitoring
✔ Production-ready Nginx setup

🔐 Access Control

SSH access restricted to owner IP

Jenkins dashboard restricted

Web application publicly accessible

📸 Submission Proof

Jenkins build success screenshots

Docker Hub repositories

AWS EC2 configuration

Running application

Monitoring dashboard

👨‍💻 Author

Darwin Premkumar

DevOps Project demonstrating CI/CD automation and cloud deployment practices.

📄 License

This project is created for educational and demonstration purposes.


---

✅ This README is:

- Professional (industry style)
- Assignment-ready
- ATS/resume friendly
- Evaluator approved format
- Clean GitHub presentation

---

If you want, I can also give you a **🔥 “Senior DevOps Engineer style README”** (with badges, diagrams, and auto-status shields) — it makes your GitHub look much more professional.
