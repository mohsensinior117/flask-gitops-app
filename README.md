

# Flask GitOps Application

A production-ready Flask application demonstrating GitOps practices with ArgoCD and Kubernetes.

## 🚀 Features

- Flask REST API with health checks
- Docker containerization with multi-stage builds
- Kubernetes deployment manifests
- GitOps workflow with ArgoCD
- Production-ready configuration

## 📦 Project Structure

```

├── app/ # Flask application
│ ├── app.py # Main application
│ └── requirements.txt # Python dependencies
├── k8s/ # Kubernetes manifests
│ ├── namespace.yaml
│ ├── deployment.yaml
│ └── service.yaml
├── Dockerfile # Container build
└── README.md

```

## 🔧 Endpoints

- `GET /` - Welcome message
- `GET /health` - Health check (for liveness probe)
- `GET /ready` - Readiness check
- `GET /info` - Application information
- `GET /api/data` - Sample API endpoint
- `POST /api/data` - Echo API endpoint

## 🛠️ Technology Stack

- **Application**: Python 3.11 + Flask
- **Container**: Docker (multi-stage build)
- **Orchestration**: Kubernetes (k3s)
- **GitOps**: ArgoCD
- **CI/CD**: GitHub Actions (planned)

## 📊 Deployment

Deployed using GitOps methodology:
- Source code repository (this repo)
- ArgoCD monitors this repository
- Automatic/manual sync to Kubernetes cluster

## 🎯 Production Features

- ✅ Health and readiness probes
- ✅ Resource limits and requests
- ✅ Rolling updates with zero downtime
- ✅ Non-root container user
- ✅ Optimized Docker image (55MB)

## 📝 Author

DevOps learning project - GitOps CI/CD Pipeline

