# 🐳 Flask on Azure Kubernetes Service (AKS) with CI/CD 🚀

This project demonstrates deploying a **containerized Flask application** on **Azure Kubernetes Service (AKS)** with a complete **CI/CD pipeline using GitHub Actions**.

## 📌 Project Overview

- 🧱 Build a Flask web app
- 🐳 Containerize it with Docker
- ☁️ Push image to Azure Container Registry (ACR)
- ⚙️ Deploy on AKS using Kubernetes manifests
- 🔄 Automate the pipeline using GitHub Actions

---

## 🧰 Tools & Technologies

| Tool              | Purpose                         |
|-------------------|----------------------------------|
| **Flask**         | Python web framework             |
| **Docker**        | Containerization of the app      |
| **Azure ACR**     | Private Docker image registry    |
| **Azure AKS**     | Kubernetes hosting               |
| **Terraform**     | Infrastructure provisioning      |
| **GitHub Actions**| CI/CD automation                 |

---

## 🚀 Live Demo

🖥️ App is deployed and accessible at:  
[http://108.141.245.46](http://108.141.245.46)

> _(Replace with domain later if added via Ingress)_

---

## ⚙️ Infrastructure Setup (Terraform)

Provisioned using Terraform:

- ✅ Resource Group
- ✅ AKS Cluster
- ✅ Azure Container Registry (ACR)

---

## 🛠️ Deployment Pipeline (GitHub Actions)

On every push to `main`:
- Docker image is built
- Image is pushed to ACR
- AKS deployment is updated using `kubectl set image`

GitHub Actions workflow:  
`.github/workflows/deploy.yml`

---

## 📂 Project Structure

flask-aks-app/
├── app.py
├── Dockerfile
├── deployment.yaml
├── service.yaml
├── main.tf # Terraform: RG + AKS + ACR
├── terraform.tfvars
├── variables.tf
└── .github/
└── workflows/
└── deploy.yml



---

## 🧠 What I Learned

- Deploying containers to Kubernetes using AKS
- Building infrastructure as code using Terraform
- Configuring CI/CD with GitHub Actions
- Managing secrets and service principals securely
- Debugging AKS + ACR + LoadBalancer setup end-to-end

---

---

## 🤝 Connect with Me

👤 [Haidi Zakaria on LinkedIn](www.linkedin.com/in/haidi-zakaria-bb424152)

⭐ Star this repo if you found it helpful!
