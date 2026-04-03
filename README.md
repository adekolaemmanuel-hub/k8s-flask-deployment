# Kubernetes Flask Deployment

Kubernetes manifests to deploy a Flask app on a local cluster using Minikube.

## Files
- `flask-deployment.yml` — creates 2 replicas of the Flask app
- `flask-service.yml` — exposes the app via NodePort

## Requirements
- Minikube
- kubectl

## Deploy
kubectl apply -f flask-deployment.yml
kubectl apply -f flask-service.yml
minikube service flask-service --url# k8s-flask-deployment
