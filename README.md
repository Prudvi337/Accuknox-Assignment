
This repository contains three completed tasks involving product design, Kubernetes security scanning, and containerized application deployment using Docker and GoLang. These tasks demonstrate hands-on experience with secure DevOps workflows, UI/UX design, and cloud-native deployments.

---

## 📌 Problem Statements Overview

### ✅ Problem Statement 1: Product Requirements & Wireframes

**Title**: Security Product for Container Image Scanning

**Objective**:  
Design a product that helps users scan and analyze container images to identify vulnerabilities, especially critical and high-severity issues. The goal is to help users prioritize remediation actions effectively at scale.

**Deliverables**:
- 📄 [Product Requirements Document](./PS-1/PRD.pdf)
- 🖼️ [Low-Fidelity Wireframes](./PS-1)
- 🔧 (Bonus) Development Action Items to discuss with the engineering team

---

### 🔐 Problem Statement 2: Kubernetes Security Scan

**Title**: Kubernetes Cluster Security Findings

**Objective**:  
Install a local Kubernetes cluster (using Minikube, K3s, or Kind), scan it using a tool like **Kubescape**, and generate a list of security findings.

**Deliverables**:
- ✅ Installed K8s using: `Kind`
- 🛡️ Security Tool Used: `Kubescape`
- 📦 Output: [`k8s-findings.json`](./PS-2)

---

### 📆 Problem Statement 3: GoLang DateTime Web App with K8s Deployment

**Title**: Real-Time Date & Time Web Application

**Objective**:  
Build a minimal GoLang web server that shows the current date and time, containerize it using Docker, and deploy it to a Kubernetes cluster with 2 replicas exposed over the internet.

**Deliverables**:
- 👨‍💻 [GoLang App Source Code](./PS-3)
- 🐳 Docker Image: [`prudvi77/datetime-app`](https://hub.docker.com/repository/docker/prudvi77/datetime-app)
- 📦 Kubernetes Manifests:
  - [`deployment.yaml`](./PS-3/deployment.yaml)
  - [`service.yaml`](./PS-3/service.yaml)
- 🌐 Public Access: Exposed using `NodePort` or Ingress Controller (configured on cloud or local cluster)

---

## 🚀 Quick Setup Guide (Problem 3)

### 1. Build Docker Image

```bash
docker build -t prudvi77/datetime-app .
docker push prudvi77/datetime-app
```

### 2. Deploy to Kubernetes

```bash
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
```

### 3. Access the Application

Use the NodePort or external IP (if using cloud) to access the real-time date & time app.


## 👨‍💼 Author

**Prudvi Kumar Reddy P**  
📍 Hyderabad, Telangana  
📧 prudvireddy7733@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/prudvi-kumar-reddy-5679662a5) | [GitHub](https://github.com/Prudvi337)

---

## 🏁 Conclusion

These tasks reflect a practical blend of:
- Product Thinking (Problem 1)
- Security Awareness (Problem 2)
- Full-Stack Cloud-Native DevOps (Problem 3)

This repository showcases how to approach security-first development using modern tools and practices.
