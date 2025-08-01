# 🐳 Django App with Docker & Kubernetes (Minikube)  

**A modern Django application containerized with Docker and deployed on Kubernetes using Minikube.**  

🚀 **Perfect for beginners** learning DevOps, containerization, and orchestration!  

---

## ✨ Features  

- **Dockerized** Django web app (simple HTML page)  
- **Kubernetes** deployment on **Minikube** (local cluster)  
- **Production-ready** YAML configurations  
- **Clean & modular** project structure  
- **Easy setup** for local development & testing  

---

## 🛠️ Tech Stack  

| Category       | Technologies Used |  
|---------------|------------------|  
| **Backend**   | Python 3.11, Django |  
| **DevOps**    | Docker, Kubernetes, Minikube |  
| **Config**    | YAML |  

---
myproject/
├── k8s/ # Kubernetes configs
│ ├── deployment.yaml # K8s Deployment
│ └── service.yaml # K8s Service
├── kubernetes_practicing/ # Django project
├── mainapp/ # Django App
├── Dockerfile # Docker config
├── requirements.txt # Python dependencies
└── README.md # Project docs


---

## 🚀 Quick Start  

### 🔧 Local Development  
```bash
# Clone & setup
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name

# Create & activate venv (optional)
python -m venv venv
source venv/bin/activate  # Linux/Mac
# venv\Scripts\activate  # Windows

# Install dependencies
pip install -r requirements.txt

# Run Django locally
python manage.py runserver

🐳 Docker Setup

# Build image
docker build -t buddysaran/django-k8s-app .

# Run container
docker run -p 8000:8000 buddysaran/django-k8s-app

☸️ Kubernetes (Minikube)

# Start Minikube cluster
minikube start

# Deploy to Kubernetes
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml

# Access the app
minikube service django-service

📝 Author
Huzaifa Saran
👨‍💻 DevOps & Backend Engineer | Lifelong Learner

🔹 Feedback? Open an issue or contribute! 🚀

## 📂 Project Structure  
