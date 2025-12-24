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

STEPS TO DEPLOY :
* minkube start --driver=docker 
* git clone https://github.com/VIVEKCHOWDARI10/Voting-App-Deployment.git
1. cd Voting-App-Deployment
2. kubectl apply -f .
3. kubectl get pods , kubectl get services ,kuebctl get deployments 
  ## ACESS THE APPLICATION :
4. minikube service vote --url    or
5. kubectl get nodes
6. kubectl get  node <node-name> -o wide
7. htpp://<node-ip>:<node-port>
--END--
