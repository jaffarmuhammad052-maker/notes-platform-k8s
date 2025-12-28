Kubernetes Smart Notes Application

A hands-on Kubernetes project that demonstrates deploying a simple notes application with best practices. This project covers Pods, Deployments, Services, Ingress, ConfigMaps, Secrets, Persistent Storage, Health Checks, Resource Limits, and RBAC.

📂 Project Structure
k8s-smart-notes/
├── app/                 # Deployment, Service, and Ingress YAMLs
├── config/              # ConfigMap and Secret YAMLs
├── storage/             # PersistentVolumeClaim YAML
├── security/            # ServiceAccount, Role, RoleBinding YAMLs
└── README.md

🧩 Features

Pods & Deployments: Self-healing, replicas for high availability

ConfigMaps & Secrets: Externalized configuration and sensitive data management

Services & Ingress: Stable networking and path-based routing

Persistent Storage: Data survives pod restarts

Health Checks: Liveness and readiness probes

Resource Management: CPU and memory limits

RBAC Security: Least privilege access for service accounts

⚡ Quick Start

Clone the repository

git clone https://github.com/affarmuhammad052-maker/k8s-notes-app.git
cd k8s-notes-app


Apply Configurations

kubectl apply -f config/
kubectl apply -f storage/
kubectl apply -f app/
kubectl apply -f security/


Verify

kubectl get all
kubectl get pvc
kubectl get ingress


Access the App

For Minikube, you can check Ingress IP:

minikube ip


Add notes.local to /etc/hosts pointing to Minikube IP if using Ingress.

🔧 Modules Covered
Module	Kubernetes Concept
Pods	Ephemeral nature, manual testing
Deployments	Rollouts, rollbacks, self-healing
ConfigMaps & Secrets	External configuration, sensitive data
Services & Ingress	Networking, DNS, routing
Storage	PV, PVC, StatefulSet
Resource Management	CPU/Memory requests & limits, HPA
Health Checks	Liveness, readiness, startup probes
Security & RBAC	Roles, RoleBindings, ServiceAccounts
📖 Learning Outcome

Understand how Kubernetes manages applications automatically

Apply best practices for security, networking, persistence, and scaling

Build a real DevOps-ready Kubernetes project
