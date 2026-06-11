# W3 - Kubernetes Services & Ingress Networking

## 📌 Overview

This task demonstrates Kubernetes networking using Services and Ingress. A Text-to-Speech application was exposed using ClusterIP, NodePort, LoadBalancer, and Ingress controller.

---

## 🎯 Objectives Completed

- Implemented ClusterIP Service (internal communication)
- Implemented NodePort Service (external access)
- Implemented LoadBalancer Service
- Configured Ingress for domain-based routing
- Enabled Minikube Ingress controller

---

## 🧠 Key Concepts

### ClusterIP
Internal-only service used for communication between pods.

### NodePort
Exposes application on a static port for external access.

### LoadBalancer
Provides cloud-based external access (simulated in Minikube).

### Ingress
Provides domain-based routing and single entry point for services.

---

## 🚀 Commands Used

```bash
kubectl apply -f clusterip.yaml
kubectl apply -f nodeport.yaml
kubectl apply -f loadbalancer.yaml
kubectl apply -f ingress.yaml
```
## 🌐 Access

Application accessed via:

http://tts.local

(Add entry in /etc/hosts for local resolution)

## 🏁 Status
✔ W3 Completed Successfully