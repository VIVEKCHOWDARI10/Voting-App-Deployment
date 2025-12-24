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
 * minkube start --driver=docker

CLONE THE REPO:
 * git clone https://github.com/VIVEKCHOWDARI10/Voting-App-Deployment.git

COMMANDS :
1. cd Voting-App-Deployment
2. kubectl apply -f .
3. kubectl get pods , kubectl get services ,kuebctl get deployments

 ## ACESS THE APPLICATION ##
 
OPTION 1:
4. minikube service vote --url

OPTION 2 :
5. kubectl get nodes
6. kubectl get  node  -o wide

ACCESS THE APPLICATION AT :

7. htpp://nodeip:nodeport

