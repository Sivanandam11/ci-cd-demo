# 🚀 End-to-End CI/CD Pipeline using GitHub, Jenkins, Docker & AWS EC2

## 📌 Project Overview

This project demonstrates a complete **CI/CD (Continuous Integration & Continuous Deployment)** pipeline that automatically builds and deploys a Dockerized web application whenever code is pushed to GitHub.

The pipeline is implemented using **GitHub, Jenkins, Docker, and AWS EC2**, eliminating manual deployment and ensuring faster, reliable application delivery.

---

# 🏗 Architecture

```
Developer
     │
     ▼
Modify Source Code
     │
git add .
git commit
git push
     │
     ▼
GitHub Repository
     │
GitHub Webhook
     ▼
Jenkins Pipeline
     │
Checkout Source Code
     │
Docker Build
     │
Stop Old Container
     │
Deploy New Container
     ▼
AWS EC2
     │
     ▼
Live Website
```

---

# ⚙ Technologies Used

- ☁ AWS EC2
- 🐧 Ubuntu Linux
- 🐙 Git
- 📁 GitHub
- ⚙ Jenkins
- 🐳 Docker
- 🌐 Nginx
- 🔗 GitHub Webhook
- 💻 HTML
- 🎨 CSS

---

# 📂 Project Structure

```
ci-cd-demo/
│
├── Dockerfile
├── Jenkinsfile
├── index.html
└── README.md
```

---

# 🚀 Features

✅ Automatic Build

✅ Automatic Deployment

✅ GitHub Webhook Integration

✅ Dockerized Application

✅ Jenkins Pipeline

✅ Live Deployment on AWS EC2

✅ Zero Manual Deployment

---

# 🔄 CI/CD Workflow

### Step 1

Developer updates the application.

```
nano index.html
```

---

### Step 2

Check modified files.

```
git status
```

---

### Step 3

Stage the changes.

```
git add .
```

---

### Step 4

Commit the changes.

```
git commit -m "Updated Website"
```

---

### Step 5

Push to GitHub.

```
git push origin main
```

---

### Step 6

GitHub automatically triggers Jenkins using a Webhook.

---

### Step 7

Jenkins Pipeline executes automatically.

- Checkout Source Code
- Build Docker Image
- Stop Previous Container
- Remove Previous Container
- Deploy New Container

---

### Step 8

Refresh the browser.

The updated website is now live.

---

# 🐳 Docker Commands

Build Image

```bash
docker build -t ci-cd-demo .
```

Run Container

```bash
docker run -d --name website -p 80:80 ci-cd-demo
```

View Running Containers

```bash
docker ps
```

Stop Container

```bash
docker stop website
```

Remove Container

```bash
docker rm website
```

---

# ⚙ Jenkins Pipeline

The pipeline performs the following stages.

- Checkout
- Build Docker Image
- Stop Old Container
- Remove Old Container
- Deploy New Container

---

# 🌍 Live Deployment

The application is deployed automatically on an **AWS EC2 Ubuntu Server** using Docker.

---

# 📈 Benefits

- Faster Deployment
- Continuous Integration
- Continuous Deployment
- Reduced Human Errors
- Automated Workflow
- Easy Rollback
- Scalable Architecture

---

# 📸 Demo

Whenever code is pushed to GitHub,

GitHub → Jenkins → Docker → AWS EC2

The website is updated automatically.

---

# 👨‍💻 Author

## **M. Sivanandam**

Cloud Engineer | AWS | Docker | Jenkins | GitHub | Linux

---

# ⭐ If you like this project

Give this repository a ⭐ on GitHub.

Thank you!
