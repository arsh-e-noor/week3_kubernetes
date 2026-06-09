# T3 - Pods & Deployments

## Objective

Learn Kubernetes Pods and Deployments using YAML manifests.

## Tasks Performed

- Created a Pod using pod.yaml
- Deployed Nginx container
- Verified Pod status
- Created Deployment with 3 replicas
- Verified Deployment status
- Tested Kubernetes self-healing

## Files

- pod.yaml
- deployment.yaml

## Commands Used

kubectl apply -f pod.yaml

kubectl get pods

kubectl describe pod nginx-pod

kubectl apply -f deployment.yaml

kubectl get deployments

kubectl describe deployment nginx-deployment

## Result

Successfully deployed Nginx Pod and Deployment with 3 replicas using Kubernetes YAML manifests.