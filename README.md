# 🚀 End-to-End DevOps Project -- Go Application \| Docker \| Kubernetes \| GitHub Actions \| Argo CD \| GitOps

This project showcases a **complete DevOps workflow**, starting from
containerizing a simple Go application to deploying it on Kubernetes
with a fully automated **CI/CD pipeline** using **GitHub Actions** and
**Argo CD (GitOps)**.

## 📌 Project Overview

-   Containerization with **multi-stage Docker build**
-   Secure and minimal **Distroless final image**
-   Kubernetes deployment using **Deployment**, **Service**, and
    **Ingress**
-   CI pipeline using **GitHub Actions**
-   Automated Helm chart image update
-   CD with **Argo CD (GitOps)**

## 🧱 Tech Stack

Go, Docker, Kubernetes, Helm, GitHub Actions, Argo CD, Ingress
Controller

## 📦 Containerization

Multi‑stage Dockerfile:\
- Stage 1: Build Go binary\
- Stage 2: Distroless runtime image

<img width="1900" height="925" alt="Screenshot 2025-11-06 162012" src="https://github.com/user-attachments/assets/301fc303-d862-4de2-989e-75de55ce29b3" />


## ☸️ Kubernetes Deployment

Includes: - `deployment.yaml` - `service.yaml` - `ingress.yaml`

Apply using:

    kubectl apply -f k8s/
<img width="1317" height="84" alt="Screenshot 2025-11-06 111236" src="https://github.com/user-attachments/assets/9afc7dd5-bd4c-40e7-9de4-5f3552843919" />


## ⛵ Helm Chart

Used to manage deployment configurations.\
GitHub Actions updates the image tag automatically.

## 🔄 CI (GitHub Actions)

Workflow includes: - Build Go app\
- Run code quality checks\
- Build + push Docker image\
- Update Helm chart

## 🚀 CD (Argo CD)

Argo CD auto-syncs the latest image to the cluster, enabling GitOps
workflows.

<img width="1900" height="900" alt="Screenshot 2025-11-06 163034" src="https://github.com/user-attachments/assets/70e27382-4b9c-41a0-adc1-6ead36b67023" />


## ✅ Pipeline Flow

1.  Push code to GitHub\
2.  GitHub Actions builds → scans → pushes image → updates Helm chart\
3.  Argo CD deploys latest version to Kubernetes

< img width="1909" height="695" alt="Screenshot 2025-11-06 124954" src="https://github.com/user-attachments/assets/bf61fd77-4f21-44b3-a322-9ed9b32eb8f2" />






<img width="1883" height="966" alt="Screenshot 2025-11-06 162906" src="https://github.com/user-attachments/assets/c71ed387-6a1c-4ff3-b2a0-c13ba9e979c1" />



