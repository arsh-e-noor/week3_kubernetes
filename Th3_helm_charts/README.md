# Week 3 - Kubernetes Orchestration (TH3 Helm Package Manager)

## 📌 Overview

This task focused on learning and using Helm, the Kubernetes package manager. A custom Helm chart was created for the Text-to-Speech web application and deployed successfully on a local Minikube Kubernetes cluster.

---

## 🎯 Objectives Completed

* Installed and configured Helm
* Explored Helm chart structure
* Created a custom Helm chart for the application
* Configured application deployment using Helm values
* Deployed the application on Minikube using Helm
* Verified Kubernetes resources created by Helm

---

## 🛠 Tools Used

* Kubernetes
* Minikube
* Helm v3
* Docker

---

## 📦 Application

**Text-to-Speech Web Application**

Docker Image:

```bash
arshen00r/text-to-speech:v1
```

---

## 🚀 Commands Used

### Install Helm

```bash
helm version
```

### Create Helm Chart

```bash
helm create tts-app
```

### Deploy Application

```bash
helm install tts-release ./tts-app
```

### Verify Deployment

```bash
helm list

kubectl get pods

kubectl get svc

kubectl get all
```

---

## 📸 Screenshots

Screenshots captured during the deployment process:

* Helm installation verification
* Helm chart creation
* Helm deployment success
* Helm release list
* Kubernetes pods
* Kubernetes services
* Application running in browser

---

## 📁 Project Structure

```text
week3_kubernetes/
│
├── app/
│
├── T3_pods_deployments/
│
├── W3_services_networking/
│
└── TH3_helm_package_manager/
    │
    ├── tts-app/
    │   ├── Chart.yaml
    │   ├── values.yaml
    │   ├── charts/
    │   └── templates/
    │
    ├── screenshots/
    │
    └── README.md
```

---

## 🏁 Status

✅ Helm Installed

✅ Custom Helm Chart Created

✅ Application Deployed with Helm

✅ Kubernetes Resources Verified

✅ TH3 Completed Successfully
