# 🐳 Dockerized Django App Deployed with Kubernetes on Minikube

This project demonstrates a simple Django web application that has been **Dockerized** and deployed using **Kubernetes** on a local **Minikube** cluster.

## 🚀 Features

- Django web app (basic HTML page)
- Dockerfile for containerization
- Deployment & Service YAML files for Kubernetes
- Runs locally on Minikube
- Clean project structure for beginners

---

## 🛠️ Tech Stack

- Python 3.11
- Django
- Docker
- Kubernetes (Minikube)
- YAML

---

## 📦 Folder Structure

myproject(kubernetes_practicing)/
├── k8s/ # Kubernetes YAML files containing folder
  ├── deployment.yaml
  ├── service.yaml
├── kubernetes_practicing/ # Django project folder
├── mainapp/ # Django App
├── Dockerfile
├── requirements.txt
├── README.md


---

## 🧪 Local Development

```bash
# Clone the repo
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name

# (Optional) Create virtual environment
python -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run locally
python manage.py runserver

## 🐳 Docker
# Build Docker image
docker build -t buddysaran/django-k8s-app .

# Run the image
docker run -p 8000:8000 buddysaran/django-k8s-practice

☸️ Kubernetes with Minikube
bash
Copy
Edit
# Start Minikube
minikube start

# Apply Kubernetes YAMLs
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

# Open in browser
minikube service django-service
📝 Author
Huzaifa Saran
Learning DevOps, Cloud & Backend Engineering
