# 🚀 F3 AWS EKS Deployment (eksctl + Helm)

## 📌 Overview
This project demonstrates the deployment of a Kubernetes application on AWS EKS using eksctl for cluster provisioning and Helm for application deployment.

---

## 🏗️ 1. EKS Cluster Creation

```bash
eksctl create cluster \
  --name tts-eks-cluster \
  --region us-east-1 \
  --nodes 2
```
## 📦 3. Application Deployment (Helm)
cd Th3_helm_charts
helm install tts-release ./tts-app
helm upgrade --install tts-release ./tts-app
📊 4. Verify Deployment
kubectl get pods
kubectl get svc
kubectl get all

## 📌 6. Result
EKS cluster successfully created using eksctl
Worker node(s) joined cluster successfully
Application deployed using Helm chart
Kubernetes service exposed using NodePort
Pods running under deployment controller

## 🎯 Conclusion

This task successfully demonstrates AWS EKS cluster provisioning and application deployment using Helm in a Kubernetes environment.