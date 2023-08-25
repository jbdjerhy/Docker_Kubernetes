# Docker_Kubernetes
# Project Title: Docker and Kubernetes Setup for Development Environment

## Project Overview

This IT project involves setting up Docker and Kubernetes on two different environments: a Windows 10 machine (Client1) and an Ubuntu 22.04.3 LTS virtual machine. The goal is to create an isolated development environment using containers and Kubernetes to streamline the development and testing processes.

## Project Phases

### Setting up Docker on Client1 (Windows 10)
![Picture1](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/e71e233a-ad8f-462a-a45e-b3c9a28e4f0c)
1. Download Docker Desktop from the official website.
2. Install Docker 4.22.1 on the Windows machine.
![Picture2](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/9473ffee-7e8d-4b09-a8b7-5ec7184f976a)
### Installing Docker on Ubuntu 22.04.3 LTS Virtual Machine

1. Remove conflicting packages.
2. Update the package repository and install required dependencies.
3. Configure Docker's GPG key and repository.
4. Install Docker and related packages.
![Picture3](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/766bbcc7-ab23-4afb-af91-2814535a5a9d)
### Installing Minikube for Container Cluster
![Picture4](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/7aba02b9-67af-4910-a557-208d27a991b2)
1. Install necessary drivers and dependencies on Ubuntu.
2. Start Minikube on Windows, addressing any errors.
![Picture5](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/a9633d0f-4900-4fa1-bebe-6a03d645f4db)
### Configuring Kubernetes

1. Use kubectl to get default configuration information.
![Picture6](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/1996513e-97a4-47fa-ae9b-82b2a3e611a5)
3. Create two namespaces: 'development' and 'production' using namespace.yaml.
![Picture7](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/1e1ff7f0-3d1f-4b7d-876e-dad9191c1710)
![Picture8](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/2970e828-3392-48e9-a068-1d57633a41a8)
5. Remove namespaces and resources using kubectl delete and corresponding YAML files.
![Picture9](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/caadbb0d-274e-43c8-9ce4-40bbe6ee9768)
### Deploying and Managing Pods

1. Create pods in the 'development' namespace using deployment.yaml.
![Picture10](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/9be1a81f-cb82-4110-9567-e1dddbef8b59)
![Picture11](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/250a69c0-f613-4ed6-8290-30408e4d09e2)
3. Check pod event logs using kubectl describe.
![Picture12](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/fef00fc9-3194-4dfd-9436-37ea9eef3154)
5. Create a pod using the BusyBox container.
![Picture13](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/4896b3ed-3c2b-42ec-ab54-da2f3550473d)
7. Execute a shell in the BusyBox container using a bash shell (had to go back in forth between visual code and powershell).
![Picture14](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/7bce7ffe-6640-41e9-b9c5-5133710835f6)
![Picture15](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/41954a9c-8346-4ea7-b3be-53a192e1fafd)
8. Connected to one of my initial pods using the busybox on port 3000
![Picture16](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/1d6c2ba2-65f5-4748-99c1-742cf4c15d6a)
### Creating and Accessing Services

1. Create a service using service.yaml.
2. Set up Minikube tunnel.
   
![Picture17](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/790d27d6-5ec2-44b4-98e5-a83f47483518)

3. Get service information using kubectl apply.
![Picture18](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/fdea9257-cbe3-44f5-8a51-23462f6d8c0d)
4. Access the service through the browser using the "External" IP.
![Picture19](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/61b7cb9a-3bed-4f0c-acf8-1fa782dfca13)
### Cleanup

1. Clean up the Kubernetes environment by deleting resources using kubectl delete.
2. Delete Minikube to release resources.
   
![Picture20](https://github.com/jbdjerhy/Docker_Kubernetes/assets/142699688/961c1dfa-1ec4-4177-9159-f4bc10df4fea)


