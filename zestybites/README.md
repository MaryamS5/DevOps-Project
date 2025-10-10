#  Zesty Bite — CI/CD Automated Deployment

##  Project Description
Zesty Bite is a Node.js web application built and deployed using Docker containers.  
The purpose of this project is to demonstrate a **CI/CD pipeline** using **GitHub Actions**, **Docker Hub**, and **AWS EC2** for automated deployment.

---

##  CI/CD Pipeline Description
The pipeline automates the process of:
1. **Build** — Builds a Docker image for the app.
2. **Test (Optional)** — Verifies the image and code.
3. **Push** — Uploads the image to **Docker Hub**.
4. **Deploy** — Automatically deploys the new version to **AWS EC2** using SSH.

The workflow is triggered **automatically** whenever code is pushed or merged into the `main` branch.

---

##  How to Run & Deploy

### ▶ Run Locally
```bash
docker build -t zesty-bite .
docker run -d -p 3000:3000 zesty-bitegit add .
