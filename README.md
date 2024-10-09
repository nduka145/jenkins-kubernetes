# Installing jenkins on Kubernetes

## Steps to Install Jenkins on Kubernetes

### 1. Clone the repository  
Clone this Git repository to your local environment:  
git clone https://github.com/nduka145/jenkins-kubernetes.git  
cd jenkins-kubernetes  


# Jenkins on Kubernetes

This repository contains the configuration and instructions to deploy Jenkins on a Kubernetes cluster using Helm charts.

## Prerequisites

Before you begin, ensure you have the following tools installed:

- Kubernetes cluster (e.g., Minikube, AWS EKS, GKE, AKS, etc.)
- `kubectl` command-line tool
- Helm 3+
- Docker (optional, if you want to build custom Jenkins images)

## Repository Structure

- `charts/`: Contains Helm chart for Jenkins deployment.
- `jenkins-values.yaml`: Custom values for Jenkins Helm chart.
- `Jenkinsfile`: CI/CD pipeline configurations for Jenkins.
- `kubernetes/`: Kubernetes manifests (optional if using Helm).

## Steps to Install Jenkins on Kubernetes

### 1. Clone the repository

Clone this Git repository to your local environment:

```bash
git clone https://github.com/nduka145/jenkins-kubernetes.git
cd jenkins-kubernetes
