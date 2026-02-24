# Flask App Deployment with Docker & GitHub Actions 🚀

This repository demonstrates a **complete DevOps workflow** for deploying a simple Flask application on an AWS EC2 instance using **Docker** and **GitHub Actions CI/CD**.

On every push to the `main` branch, the application is automatically built and deployed to the EC2 server.

---

## 📌 Project Overview

* Flask web application
* Dockerized application
* Deployed on AWS EC2 (Ubuntu)
* CI/CD pipeline using GitHub Actions
* Automatic deployment via SSH

---

## 🛠️ Tech Stack

* **Backend:** Python, Flask
* **Containerization:** Docker
* **Cloud:** AWS EC2
* **CI/CD:** GitHub Actions
* **OS:** Ubuntu Linux

---

## ⚙️ How It Works

1. Developer pushes code to the `main` branch
2. GitHub Actions workflow is triggered
3. Workflow connects to EC2 using SSH
4. Latest code is pulled from GitHub
5. Docker image is rebuilt
6. Old container is stopped and removed
7. New container is started with updated code

---

## 🚀 Deployment Steps (High Level)

1. Launch an EC2 instance (Ubuntu)
2. Install Docker and Git
3. Clone this repository on EC2
4. Create SSH keys and configure GitHub Secrets
5. Configure GitHub Actions workflow
6. Push code to trigger auto-deployment

---

## 🌐 Accessing the Application

After successful deployment, access the application using:

```
http://<EC2_PUBLIC_IP>
```

---

## 🔐 GitHub Secrets Used

| Secret Name | Description               |
| ----------- | ------------------------- |
| `EC2_HOST`  | Public IP of EC2 instance |
| `EC2_USER`  | SSH username (ubuntu)     |
| `EC2_KEY`   | Private SSH key           |

---

## 📌 Learning Outcomes

* Understanding real-world CI/CD workflow
* Hands-on experience with Docker
* Secure SSH-based deployments
* Cloud application hosting on EC2
* Automating deployments using GitHub Actions

---

## 🧑‍💻 Author

**Muni Naveen Naidu**
B.Tech CSE | DevOps & Cloud Enthusiast

---

## ⭐ Acknowledgment

This project was created for learning and hands-on practice in DevOps and cloud deployment.
