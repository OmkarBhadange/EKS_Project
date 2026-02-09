🚀 EKS & ECK Project – Kubernetes Deployment on AWS
📌 Project Overview

This project demonstrates how to deploy a containerized application on:
Amazon EKS (Elastic Kubernetes Service)
ECK (Elastic Cloud on Kubernetes)
Using Kubernetes YAML manifests
Exposing the application via a LoadBalancer service.
The project provisions an AWS EKS cluster using eksctl, deploys an NGINX-based application, and exposes it externally using a LoadBalancer.

🏗️ Architecture

User → AWS LoadBalancer → Kubernetes Service → Deployment → NGINX Pod

Deployment manages the application pod.
Service (LoadBalancer) exposes the application externally.
EKS Cluster runs the Kubernetes control plane and worker nodes.

📂 Project Structure
EKS_Project/
│
├── deployment.yaml
├── service.yaml
└── README.md

⚙️ Prerequisites
AWS CLI configured (aws configure)
eksctl installed
kubectl installed
IAM permissions for EKS

🚀 Application Deployment
🔹 Deployment YAML

deployment.yaml
-Creates a Deployment named hello-world
-Runs nginx:latest
-Exposes container port 80
