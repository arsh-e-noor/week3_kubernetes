# Week 3 - Kubernetes Orchestration (T3: Pods & Deployments)

## 📌 Overview

This task focuses on Kubernetes workload management using Pods and Deployments. A containerized Text-to-Speech web application was deployed on a local Minikube cluster using a Docker image.

The objective was to understand how Kubernetes manages application instances and ensures high availability using replicas.

---

## 🎯 Objectives Completed

- Created and managed Kubernetes Pods
- Created Deployments with replica sets
- Understood difference between Pod and Deployment
- Deployed a containerized web application on Minikube
- Verified running pods and deployment status

---

## 🧠 Key Concepts

### Pod
Smallest deployable unit in Kubernetes that runs a single container.

### Deployment
Manages multiple replicas of Pods and ensures:
- Auto-healing
- Scaling
- Rolling updates

---

## 🚀 Application Details

- Application: Text-to-Speech Web App
- Type: Static Frontend (HTML, CSS, JS)
- Container: Nginx Alpine
- Docker Image: `tts-app:v1`

---

## 📄 Kubernetes Resources

### Pod Configuration
- Single instance of application
- Used for basic testing

### Deployment Configuration
- 3 replicas of application
- Ensures high availability
- Self-healing enabled

---

## ⚙️ Deployment Commands

```bash
kubectl apply -f pod.yaml
kubectl apply -f deployment.yaml
```
## 📁 Project Structure
week3_kubernetes/
│
└── T3_pods_deployments/
    │
    ├── pod.yaml
    ├── deployment.yaml
    ├── README.md
    │
    └── screenshots/

## 🏁 Status

✔ T3 Completed Successfully