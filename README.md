# Docker_Kubernetes
# Project Title: Docker and Kubernetes Setup for Development Environment

## Project Overview

This IT project involves setting up Docker and Kubernetes on two different environments: a Windows 10 machine (Client1) and an Ubuntu 22.04.3 LTS virtual machine. The goal is to create an isolated development environment using containers and Kubernetes to streamline the development and testing processes.

## Project Phases

### Setting up Docker on Client1 (Windows 10)

1. Download Docker Desktop from the official website.
2. Install Docker 4.22.1 on the Windows machine.

### Installing Docker on Ubuntu 22.04.3 LTS Virtual Machine

1. Remove conflicting packages.
2. Update the package repository and install required dependencies.
3. Configure Docker's GPG key and repository.
4. Install Docker and related packages.

### Installing Minikube for Container Cluster

1. Install necessary drivers and dependencies on Ubuntu.
2. Start Minikube on Windows, addressing any errors.

### Configuring Kubernetes

1. Use kubectl to get default configuration information.
2. Create two namespaces: 'development' and 'production' using namespace.yaml.
3. Remove namespaces and resources using kubectl delete and corresponding YAML files.

### Deploying and Managing Pods

1. Create pods in the 'development' namespace using deployment.yaml.
2. Check pod event logs using kubectl describe.
3. Create a pod using the BusyBox container.
4. Execute a shell in the BusyBox container using a bash shell.

### Creating and Accessing Services

1. Create a service using service.yaml.
2. Set up Minikube tunnel.
3. Get service information using kubectl apply.
4. Access the service through the browser using the "External" IP.

### Cleanup

1. Clean up the Kubernetes environment by deleting resources using kubectl delete.
2. Delete Minikube to release resources.

## Project Documentation

Ensure to create detailed documentation for the setup process, including any errors encountered and how they were resolved. This documentation will serve as a reference for future use and for sharing knowledge within your team.

