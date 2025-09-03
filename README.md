# 🚀 Build & Publish Docker Image using GitHub Actions

This project demonstrates how to build a simple **Flask application**, containerize it with **Docker**, and automatically publish the image to **DockerHub** using **GitHub Actions**.

---

## 📌 Project Overview
- A basic Python Flask app (`app.py`)
- Dockerized using a `Dockerfile`
- GitHub Actions workflow to:
  - Build Docker image
  - Authenticate to DockerHub
  - Push image on every commit to `main`

---

## 🛠️ Tech Stack
- **Python 3.9 (Flask)**
- **Docker**
- **GitHub Actions**
- **DockerHub**

---

## ⚙️ Setup & Run Locally

### 1. Clone the repository
```bash
git clone https://github.com/Raghavachari93/publish-docker-image.git
cd publish-docker-image

2. Build the Docker image
docker build -t flask-docker-app .

3. Run the container
docker run -p 5000:5000 flask-docker-app


Now open 👉 http://localhost:5000
 in your browser.

🚀 Using Pre-Built Image from DockerHub

Instead of building locally, you can pull the pre-built image:

docker pull docker-username/flask-docker-app:latest
docker run -p 5000:5000 docker-username/flask-docker-app:latest

🔄 CI/CD with GitHub Actions

Workflow file: .github/workflows/docker-image.yml

On every push to main:

Code is checked out

DockerHub login happens using GitHub Secrets (DOCKER_USERNAME, DOCKER_PASSWORD)

Image is built & pushed to DockerHub (docker-username/flask-docker-app:latest)

🔑 GitHub Secrets Configuration

Add the following secrets in your GitHub repo:

DOCKER_USERNAME → your DockerHub username

DOCKER_PASSWORD → your DockerHub Access Token
