# 🚀 Docker + Kubernetes Java Microservices Project

## 📌 Project Overview

This project demonstrates a complete DevOps workflow using Docker and Kubernetes with Java Spring Boot microservices.

The application consists of 3 independent microservices:

* Product Catalogue Service
* Stock Manager Service
* Shopfront Service

All services are containerized using Docker and deployed into a Kubernetes cluster using Minikube.

---

# 🛠️ Technologies Used

* Java Spring Boot
* Docker
* Kubernetes
* Minikube
* Maven
* Ubuntu Linux

---

# 📂 Microservices

| Service           | Description                 | Port |
| ----------------- | --------------------------- | ---- |
| Product Catalogue | Product information service | 8020 |
| Stock Manager     | Inventory & stock service   | 8030 |
| Shopfront         | Frontend application        | 8010 |

---

# ⚙️ Features

✅ Dockerized Java microservices
✅ Kubernetes Deployments & Services
✅ NodePort exposure
✅ Liveness probes
✅ Docker Hub image registry
✅ Minikube local cluster setup
✅ Microservices communication

---

# 🐳 Docker Workflow

## Build Maven Package

```bash
mvn clean package -DskipTests
```

## Build Docker Image

```bash
docker build -t sakibdevops/productcatalogue:v1 .
```

## Push Docker Image

```bash
docker push sakibdevops/productcatalogue:v1
```

---

# ☸️ Kubernetes Deployment

## Apply Kubernetes YAML Files

```bash
kubectl apply -f kubernetes/productcatalogue-service.yaml
kubectl apply -f kubernetes/stockmanager-service.yaml
kubectl apply -f kubernetes/shopfront-service.yaml
```

## Verify Pods

```bash
kubectl get pods
```

## Verify Services

```bash
kubectl get svc
```

---

# 🚀 Running the Project

## Start Minikube

```bash
minikube start --driver=docker
```

## Open Services

```bash
minikube service productcatalogue
minikube service stockmanager
minikube service shopfront
```

---

# 📊 Kubernetes Concepts Used

* Deployment
* Service
* NodePort
* Pods
* ReplicaSets
* Liveness Probes

---

# 🔥 Challenges Solved

* Docker authentication issues
* ImagePullBackOff troubleshooting
* CrashLoopBackOff debugging
* Java compatibility issues
* Kubernetes networking

---

# 📸 Architecture Diagram

Add your project architecture image here.

```md
![Architecture](images/project-architecture.png)
```

---

# 🎯 Learning Outcome

Through this project I learned:

* Real-world DevOps workflow
* Docker image management
* Kubernetes deployments
* Debugging production-like issues
* Microservices deployment architecture

---

# 👨‍💻 Author

## S. M. Mahedi Hasan

Aspiring DevOps Engineer focused on:

* Docker
* Kubernetes
* Linux
* Cloud
* Automation
* Microservices

---

# ⭐ Support

If you like this project, give it a ⭐ on GitHub.


<img width="1536" height="1024" alt="Java_microservice_kubernetes" src="https://github.com/user-attachments/assets/fac9cb06-2fe6-42b4-8d6e-fa2946040a29" />


Source Code Credit: https://github.com/danielbryantuk/oreilly-docker-java-shopping/
