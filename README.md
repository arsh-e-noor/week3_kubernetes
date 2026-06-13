# 🚀 Week 3 - AWS EKS Deployment & Kubernetes (DevOps Internship)
## 📌 Repository Overview

This repository contains Week 3 DevOps internship tasks focused on Kubernetes, AWS EKS, Helm charts, and deploying applications on a managed Kubernetes cluster using eksctl.

The main goal of this week was to create an EKS cluster and deploy an application using Kubernetes and Helm.

## 🧠 Learning Objectives

By completing this week, I learned:

Kubernetes architecture and core concepts
Creating AWS EKS clusters using eksctl
Working with managed node groups
Understanding pods, deployments, and services
Debugging pod lifecycle issues (Pending/Running states)
Using Helm charts for Kubernetes deployments
Deploying applications on AWS EKS
## 📂 Folder Structure
week3_kubernetes/
│
├── M3_setup/
├── T3_pods_deployments/
├── W3_services_networking/
├── Th3_helm_charts/
├── F3_aws_eks_deployment/
└── README.md
## ☁️ F3 - AWS EKS Deployment
### 📌 Objective

Create and manage a Kubernetes cluster using AWS EKS and deploy a sample application.

### 📌 Steps Performed
Created EKS cluster using eksctl
Created managed node group (EC2 worker nodes)
Installed required Kubernetes addons:
CoreDNS
kube-proxy
vpc-cni
metrics-server
Configured kubeconfig using AWS CLI
Verified cluster connectivity using kubectl
### 📌 Commands Used
eksctl create cluster --name tts-eks-cluster --region us-east-1 --nodes 2

aws eks update-kubeconfig --name tts-eks-cluster --region us-east-1

kubectl get nodes
kubectl get pods -A
## 📌 Outcome
EKS cluster successfully created
Worker node joined cluster successfully
Kubernetes control plane and node communication established
## 📦 T3 - Pods & Deployments
### 📌 Objective

Deploy Kubernetes Pods and Deployments on EKS cluster.

### 📌 Steps Performed
Created deployment YAML
Deployed application using Kubernetes deployment
Verified pod status and replica sets
Observed pod lifecycle behavior
### 📌 Outcome
Deployment created successfully
Pods were scheduled but initially showed Pending
Learned debugging of scheduling and resource allocation issues
## 🌐 W3 - Kubernetes Services & Networking
### 📌 Objective

Expose Kubernetes applications using different service types.

### 📌 Services Used
ClusterIP
NodePort
LoadBalancer
### 📌 Steps Performed
Created service YAML files
Exposed deployment using NodePort service
Verified service using kubectl
### 📌 Outcome
Successfully exposed application inside cluster
Learned how networking works in Kubernetes
## 📊 Th3 - Helm Charts
### 📌 Objective

Deploy application using Helm package manager.

### 📌 Steps Performed
Used existing Helm chart (tts-app)
Installed Helm release on EKS cluster
Upgraded Helm release
Verified pods and services created by Helm
### 📌 Commands Used
helm install tts-release ./tts-app

helm upgrade --install tts-release ./tts-app

kubectl get pods
kubectl get svc
kubectl get all
### 📌 Outcome
Helm release successfully deployed
Kubernetes objects created automatically via templates
Learned Helm chart structure and usage
### ⚙️ Tools & Technologies Used
AWS EKS
eksctl
Kubernetes (kubectl)
Helm
AWS CLI
Ubuntu
CloudFormation (backend for EKS provisioning)
## 🚀 Final Outcome

This project demonstrates a complete Kubernetes deployment workflow on AWS:

eksctl → AWS EKS Cluster → Node Group → Kubernetes → Helm Deployment → Running App
## 📸 Evidence

The repository includes screenshots and logs showing:

EKS cluster creation
Node group joining cluster
Pod and deployment status
Service exposure
Helm installation and upgrade
## 🎯 Conclusion

This week provided hands-on experience with AWS EKS and Kubernetes deployments. It helped me understand how real-world cloud-native applications are deployed using managed Kubernetes and Helm automation.

# 👩‍💻 Author

Arsh E Noor
Week 3 - AWS EKS Deployment & Kubernetes