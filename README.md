# CI/CD Pipeline with GitHub Actions & Docker

## 🚀 Project Overview
This project demonstrates a fully automated **CI/CD pipeline** using **GitHub Actions** and **Docker**, automating the build, test, and deployment of a static HTML + Bootstrap website locally without any cloud infrastructure.

---

## 🎯 Objective
Build a CI/CD pipeline that:
- Builds a Docker image
- Pushes the image to Docker Hub
- Deploys the container locally using a Virtual Machine (VM)

---

## 🛠 Tools Used
- GitHub Actions
- Docker & Docker Hub
- Local Virtual Machine (VM)
- HTML & Bootstrap Template from https://templatemo.com/

---

## ⚡ Features
- Automated workflow triggered on `main` branch push
- Secure Docker Hub login using GitHub Secrets
- Build & Push Docker image
- Deploy locally for demonstration using a local VM

---

## ✅ Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/GouravSharma007/Github-Actions-Docker.git
   ```
Set up Docker Hub secrets in your GitHub repo: Follow this path GitHub Repo> Settings> Secrets and Variables> Actions> New Repository Secret.

- DOCKER_USERNAME

- DOCKER_PASSWORD

The pipeline automatically triggers on every commit to main.
The image is built and pushed to Docker Hub.

To deploy locally on your VM:
```bash
docker pull gourav0/ci-cd-demo:latest
docker run -d -p 8080:80 gourav0/ci-cd-demo
Search http://localhost:8080 in your browser to view the deployed website.
```
---

## 📸 Screenshots
1. Workflow of GitHub Action pipeline
<img width="891" height="621" alt="Image" src="https://github.com/user-attachments/assets/c8aaad35-804a-4493-96fd-e67c9fbe4cda" />


2. This is an image of docker hub repo where I have my docker image
<img width="1230" height="721" alt="Image" src="https://github.com/user-attachments/assets/c7cf72b8-f665-4ffa-bd61-df4242692e60" />


3. Search localhost:8080 on any web browser you have
<img width="1912" height="955" alt="Image" src="https://github.com/user-attachments/assets/fb253fc0-3f58-4e17-b346-fc74fe40fa00" />

---

## ✅ Conclusion
This project demonstrates how to automate the development and deployment process using GitHub Actions and Docker. It shows a simple, efficient, and consistent way to build and deploy a static website locally, removing the need for manual operations.

---

## 🔗 Docker Image Link
```bash
https://hub.docker.com/r/gourav0/ci-cd-demo
```
