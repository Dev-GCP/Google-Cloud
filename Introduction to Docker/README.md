# 🐳 Introduction to Docker

Welcome to this hands-on lab on **Docker**, designed for beginners in cloud and container technology.

---

## 📌 Lab Objectives

- ✅ Understand the role of Docker
- ✅ Install Docker on your system
- ✅ Pull and run a Docker container
- ✅ Explore basic Docker commands
- ✅ Push your own image to Docker Hub

---

## 🧰 Prerequisites

- A system with Docker installed (or install instructions included)
- Internet connection
- Basic command line knowledge

---

## 🛠️ Task 1: Install Docker

### For Ubuntu/Linux:

```bash
sudo apt update
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
docker --version
```
## 🛠️ Task 2:  Pull and Run a Docker Image
```bash
docker pull hello-world
docker run hello-world

```
## 🛠️ Task 3: Run a Web Server (Nginx)
```bash
docker pull nginx
docker run -d -p 8080:80 nginx
```
Open your browser and visit:
👉 http://localhost:8080

🧹 Task 4: Clean Up
```bash
docker ps -a           # List all containers
docker stop <container_id>
docker rm <container_id>
docker image ls        # List images
docker rmi <image_id>

