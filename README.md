# 🚀 Kubernetes Test Application

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python" />
  <img src="https://img.shields.io/badge/Flask-3.0-lightgreen?style=flat-square&logo=flask" />
  <img src="https://img.shields.io/badge/Docker-Enabled-blue?style=flat-square&logo=docker" />
  <img src="https://img.shields.io/badge/Kubernetes-Ready-blue?style=flat-square&logo=kubernetes" />
</p>

A simple yet elegant **Flask web application** to demonstrate how to **Dockerize** and run workloads on **Kubernetes** using Minikube.  
This project is perfect for **beginners learning Kubernetes, Docker, and containerized app deployment**.

---

## 🛠️ Tech Stack

| Layer             | Technology |
|-------------------|------------|
| **Frontend**      | HTML, CSS (modern, responsive UI) |
| **Backend**       | Python Flask |
| **Containerization** | Docker |
| **Orchestration** | Kubernetes (Minikube) |

---

## 📂 Project Structure

```text
K8s-Demo-Project/
├── app.py               # Flask backend code
├── requirements.txt     # Python dependencies
├── Dockerfile           # Docker build instructions
├── templates/           # HTML templates
│   └── index.html
├── static/              # CSS styles
│   └── styles.css
├── k8s/                 # Kubernetes manifests
│   ├── deployment.yaml
│   └── service.yaml
└── README.md            # You are here
```
---

## ⚡ Getting Started (Local)

1. Clone the repository  
   `git clone https://github.com/<your-username>/K8s-Demo-Project.git && cd K8s-Demo-Project`

2. Install dependencies  
   `pip install -r requirements.txt`

3. Run locally  
   `python app.py`  
   Visit: **http://localhost:5001**

---

## 🐳 Running with Docker

1. Build the image  
   `docker build -t k8s-test-app .`

2. Run the container  
   `docker run --rm -p 5001:5001 --name k8s-test k8s-test-app`  
   Visit: **http://localhost:5001**

---

## ☸ Deploying on Minikube

1. Start Minikube  
   `minikube start`

2. Load your Docker image into Minikube  
   `minikube image load k8s-test-app`

3. Apply Kubernetes manifests  
   `kubectl apply -f k8s/deployment.yaml && kubectl apply -f k8s/service.yaml`

4. Access the app  
   `minikube service k8s-test-service`

---

## 💡 Learning Objectives

✅ Understand how to **containerize** a Python Flask app  
✅ Learn to **build and run Docker images**  
✅ Deploy and manage the app on **Kubernetes with Minikube**  
✅ Explore **Kubernetes Deployments & Services** basics  

---

## 🤝 Contributing
Feel free to fork this project, submit pull requests, or open issues to improve the code or documentation.

---

## 📜 License
This project is licensed under the **MIT License**.

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/<your-username>">Your Name</a>
</p>
