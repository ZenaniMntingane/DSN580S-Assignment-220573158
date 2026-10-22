# DSN580S-Assignment-220573158
DSN580S Assignment 2: Minikube on AWS
Student Information
Student Number: 220573158
Module Name: Distributed Systems and Software Defined networks
Module code: DSN580S
Assignment: Kubernetes with Minikube on AWS EC2

Project Overview
This project demonstrates the deployment and management of a single-node Kubernetes cluster using Minikube on an AWS EC2 Ubuntu instance. Docker was used as the container runtime, Kubernetes resources were deployed using YAML manifests, and Portainer was configured to monitor the environment.

Environment Details
Amazon Machine Image: Ubuntu server LTS, 64-bit
Instance type: T3. medium
Key: 220573158
Space 30 GB

Installation Steps
Update Ubuntu
sudo apt upgrade -y

Task 2
2.1 Install Docker
Run this code in Shell
sudo apt install docker.io -y
sudo systemctl enable docker
sudo systemctl start docker
docker --version 
2.2  Install kubectl 
Run this code on a buntu terminal 
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
chmod +x kubectl
sudo mv kubectl /usr/local/bin/
kubectl version --client

2.3 Minikube Installation
Run this code on a buntu terminal 
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
minikube version

Start Minikube
Run this code on a terminal
minikube start --driver=docker

