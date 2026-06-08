# Week 3 - Kubernetes Orchestration (M3 Setup)

## 📌 Overview

This module covers Kubernetes fundamentals using a local Minikube cluster. The goal was to understand Kubernetes architecture and successfully deploy and verify a working cluster on a local machine using Docker as the driver.

---

## 🎯 Objectives Completed

* Understood Kubernetes architecture (Control Plane & Worker Nodes)
* Installed and configured kubectl
* Installed and configured Minikube
* Started a local Kubernetes cluster using Docker driver
* Verified cluster health and system components

---

## 🧠 Kubernetes Architecture Summary

### Control Plane (Master Node)

Responsible for managing the cluster:

* API Server → Entry point for all requests
* Scheduler → Assigns pods to nodes
* Controller Manager → Maintains desired state
* etcd → Key-value store for cluster data

### Worker Node

Runs application workloads:

* Kubelet → Communicates with control plane
* Container Runtime → Runs containers (Docker)
* Kube Proxy → Handles networking

---

## 📦 Key Kubernetes Concepts

### Pod

Smallest deployable unit in Kubernetes that runs one or more containers.

### Deployment

Ensures desired number of pod replicas are always running.

### Service

Exposes pods to network traffic.

Types:

* ClusterIP (internal access)
* NodePort (external access via port)
* LoadBalancer (cloud exposure)

---

## ⚙️ Tools Used

* Docker
* kubectl
* Minikube (v1.38.1)

---

## 🚀 Setup Commands Used

```bash
# Check Docker
docker --version
docker ps

# Install kubectl
curl -LO https://dl.k8s.io/release/stable.txt
chmod +x kubectl
sudo mv kubectl /usr/local/bin/

# Verify kubectl
kubectl version --client

# Install Minikube
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube

# Start cluster
minikube start --driver=docker

# Verify cluster
kubectl get nodes
kubectl cluster-info
kubectl get pods -A
```

---

## 📸 Evidence / Screenshots

Screenshots are stored in:

```
m3_setup/screenshots/
```

Include:

* 01-minikube-start.png → Minikube cluster startup success
* 02-get-nodes.png → Kubernetes node status
* 03-cluster-info.png → Cluster information output
* 04-get-pods.png → System pods running

---

## 📁 Project Structure

```
week3_kubernetes/
│
│
└── m3_setup/
    │
    └── screenshots/
        ├── 01-minikube-start.png
        ├── 02-kubectl-version.png
        ├── 03-minikube-version.png
        └── 04-commands.png
    │
    └── README.md
```

---


## 🏁 Status

✔ M3 Completed Successfully
