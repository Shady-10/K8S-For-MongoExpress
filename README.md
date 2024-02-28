
MongoDB and MongoDB Express Cluster Deployment
This repository contains Kubernetes YAML files to deploy a MongoDB cluster and MongoDB Express for easy management.

Prerequisites
Minikube
kubectl
Deployment
Start Minikube:

sh
Copy code
minikube start
Deploy MongoDB:

sh
Copy code
kubectl apply -f mongodb-deployment.yaml
Deploy MongoDB Express:

sh
Copy code
kubectl apply -f mongoexpress-deployment.yaml
Access MongoDB Express:
Get the URL for MongoDB Express service:

sh
Copy code
minikube service mongoexpress --url
Open the URL in a web browser to access MongoDB Express.

To attach an external IP for the MongoDB Express service, run:

sh
Copy code
minikube service mongoexpress
