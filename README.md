# 🚀 DevOps CI/CD Project – Docker + Kubernetes + Jenkins + Ansible

## 📌 Project Overview

This project demonstrates a complete DevOps lifecycle for deploying a static website application using:

- GitHub (Version Control)
- Docker (Containerization)
- Jenkins (CI/CD Pipeline)
- Kubernetes (Container Orchestration)
- Ansible (Configuration Management)

The application is automatically built, containerized, pushed to Docker Hub, and deployed on a Kubernetes cluster.

---

## 🏗️ Architecture
GitHub → Jenkins → Docker Build → Docker Hub → Kubernetes Deployment

---

## 🖥️ Infrastructure Setup

The project uses **4 EC2 instances on AWS**:

| Server | Role |
|-------|------|
| Jenkins Server | CI/CD Build Server |
| Master Node | Kubernetes Control Plane |
| Worker Node 1 | Kubernetes Worker |
| Worker Node 2 | Kubernetes Worker |

---

## ⚙️ Tools & Technologies Used

- Git & GitHub
- Docker
- Jenkins
- Kubernetes (kubeadm cluster)
- Ansible
- AWS EC2 (Ubuntu)

---

## 📁 Project Structure

website1/
├── Dockerfile
├── Jenkinsfile
├── deployment.yaml
├── service.yaml
├── index.html
├── images/
└── ansible/
├── inventory.ini
├── site.yml
├── jenkins.yml
└── docker-k8s.yml

---

## 🐳 Docker Setup

### Build Image
```bash
docker build -t darshandarshu/website:latest .
