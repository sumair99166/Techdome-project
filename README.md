# Techdome Project

A simple Next.js application containerized with Docker and deployable on Kubernetes.  

---

## Project Overview

This project demonstrates a **Next.js app** with **Docker** and **Kubernetes** setup, ready for CI/CD pipelines.

---

## Local Setup

1. Clone the repository:

```bash
git clone https://github.com/sumair99166/Techdome-project.git
cd Techdome-project
Install dependencies:

bash
Copy code
npm ci
Build and run locally:

bash
Copy code
npm run build
npm start
Open http://localhost:3000 in your browser.

Docker Setup
Build Docker image:

bash
Copy code
docker build -t techdome-app .
Run container:

bash
Copy code
docker run -p 3000:3000 techdome-app
Open http://localhost:3000 in your browser.

Kubernetes Deployment
Make sure Kubernetes is running (Docker Desktop/Minikube).

Apply manifests:

bash
Copy code
kubectl apply -f k8s/deployment.yml
kubectl apply -f k8s/service.yml
Check pods and service:

bash
Copy code
kubectl get pods
kubectl get svc
Port-forward to access the app:

bash
Copy code
kubectl port-forward svc/techdome-service 3000:3000
Open http://localhost:3000 in your browser.

