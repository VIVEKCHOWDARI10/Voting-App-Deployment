# Kubernetes Voting App Deployment #

Description:
This project demonstrates the deployment of a multi-tier voting application on Kubernetes using Minikube.  
The application consists of:
* Frontend voting app
* Backend worker service
* Redis queue
* PostgreSQL database
* Result app

The project showcases the use of Pods, Deployments, and Services in a Kubernetes cluster and how to access the app locally using Minikube.



## Technologies Used ##

* Kubernetes (Minikube)
* Docker
* YAML manifests
* kubectl commands
* Linux

## STEPS TO DEPLOY ##

START THE MINIKUBE: 
 * minikube start --driver=docker

CLONE THE REPO:
```bash
git clone https://github.com/VIVEKCHOWDARI10/Voting-App-Deployment.git
```

COMMANDS :
```bash
cd Voting-App-Deployment
```
```bash
 kubectl apply -f .
```
```bash 
kubectl get pods , kubectl get services ,kubectl get deployments
```

 ## ACCESS THE APPLICATION ##
 
OPTION 1:
```bash
minikube service vote --url
```

OPTION 2 :
```bash
 kubectl get nodes
```
```bash
kubectl get  node  -o wide
```
ACCESS THE APPLICATION AT :

http://nodeip:nodeport

