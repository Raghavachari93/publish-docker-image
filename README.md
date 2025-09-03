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
