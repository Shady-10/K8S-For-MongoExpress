# MongoDB and MongoDB Express Cluster Deployment

This repository contains Kubernetes YAML files to deploy a MongoDB cluster and MongoDB Express for easy management.

## Prerequisites

- [Minikube](https://minikube.sigs.k8s.io/docs/start/)
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)

## Deployment

1. Start Minikube:
   ```sh
   minikube start

Deploy MongoDB:
kubectl apply -f mongodb-deployment.yaml


Deploy MongoDB Express:
kubectl apply -f mongoexpress-deployment.yaml


Access MongoDB Express:
Get the URL for MongoDB Express service:
minikube service mongoexpress --url


To attach an external IP for the MongoDB Express service, run:
minikube service mongoexpress
