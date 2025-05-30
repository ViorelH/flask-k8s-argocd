# Flask Kubernetes Deployment with ArgoCD

This repository contains Kubernetes manifests for deploying a simple Flask app via GitOps using ArgoCD.

## Project Structure

k8s/
├── deployment.yaml
└── service.yaml

markdown
Copy
Edit

## How it works

- ArgoCD automatically pulls these manifests from GitHub and applies them to the Kubernetes cluster.
- Any time changes are pushed to GitHub, ArgoCD syncs them automatically.

## Useful Commands

- Build Docker image:

  docker build -t flask-k8s:latest .

Apply manifests manually (if needed):

kubectl apply -f k8s/

Next Steps

Publish image to Docker Hub or ECR for cluster-wide deployments.

Use ArgoCD's auto-sync feature for full GitOps automation.

Author

ViorelH - Project 7: GitOps with ArgoCD
