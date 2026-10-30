# 🚀 HOTSTAR – END-TO-END DEVOPS CI/CD PROJECT

## 📌 Project Overview

This project demonstrates an end-to-end DevOps CI/CD pipeline for deploying a Hotstar demo application using modern DevOps tools and AWS Cloud infrastructure.

The project integrates Git, GitHub, Jenkins, Maven, Docker, Docker Hub, Linux, AWS EC2, AWS S3 and Kubernetes to automate application building, containerization, and deployment.

## 🏗️ Project Architecture

mermaid
flowchart TD
    A[Developer] --> B[Git]
    B --> C[GitHub Repository]
    C --> D[Jenkins CI/CD]
    D --> E[Maven Build]
    E --> F[Java Application JAR]
    F --> G[Docker Build]
    G --> H[Docker Image]
    H --> I[Docker Hub]
    I --> J[AWS EC2 Linux]
    J --> K[Kubernetes K3s]
    K --> L[Deployment]
    L --> M[Pods]
    M --> N[Hotstar Application]

    O[AWS S3 Storage] -.-> J


## 🧰 Technologies & Tools Used

| Technology | Purpose |
|---|---|
| Linux | Operating System |
| AWS | Cloud Infrastructure |
| EC2 | Compute Instance |
| S3 | Cloud Storage |
| Git | Version Control |
| GitHub | Source Code Management |
| Jenkins | CI/CD Automation |
| Java | Application Development |
| Maven | Build Automation |
| Docker | Containerization |
| Docker Hub | Container Image Registry |
| Kubernetes | Container Orchestration |
| K3s | Lightweight Kubernetes |
| kubectl | Kubernetes Management |

## 🔄 CI/CD Pipeline Workflow

1. Developer pushes source code to GitHub.
2. Git manages source code versioning.
3. Jenkins executes the CI/CD pipeline.
4. Maven builds and packages the Java application.
5. Docker creates the application container image.
6. Docker image is pushed to Docker Hub.
7. Kubernetes pulls the Docker image.
8. Kubernetes Deployment manages application Pods.
9. Application runs inside Kubernetes Pods.

## ☁️ AWS Infrastructure

### Amazon EC2
- Linux-based cloud compute environment.
- Hosts the DevOps project environment.
- Used for Docker and Kubernetes operations.

### Amazon S3
- Cloud object storage.
- Used for project-related storage requirements.

## 🐳 Docker & Docker Hub

Docker is used to containerize the Hotstar application.

Docker Hub Image:

natscloud/hotstar:latest

Pull Docker Image:

bash
docker pull natscloud/hotstar:latest


Docker Hub Repository:

https://hub.docker.com/r/natscloud/hotstar

## ☸️ Kubernetes Deployment

Kubernetes is used to deploy and manage application containers.

Kubernetes Commands:

Check Nodes:

bash
kubectl get nodes


Check Pods:

bash
kubectl get pods -o wide


Check Deployments:

bash
kubectl get deployments


Check Services:

bash
kubectl get svc


Check Pod Details:

bash
kubectl describe pod <pod-name>


Check Application Logs:

bash
kubectl logs <pod-name>


Apply Kubernetes Configuration:

bash
kubectl apply -f k8s/


## ⚙️ Maven Build

Build the Java application using Maven:

bash
mvn clean package


Maven generates the application JAR file inside the target directory.

## 📁 Project Structure

text
HOTSTAR-DEVOPS-PROJECT/
│
├── src/
├── k8s/
│   ├── deployment.yaml
│   └── service.yaml
│
├── Dockerfile
├── Jenkinsfile
├── pom.xml
├── .gitignore
└── README.md


Update this structure according to the actual repository files.

## 🔐 Security Best Practices

- Never upload AWS Access Keys or Secret Keys.
- Store credentials securely in Jenkins Credentials.
- Use Docker Hub access tokens.
- Protect SSH private keys.
- Avoid hardcoding sensitive information.

## 📸 Project Screenshots

Add your actual project screenshots here:

- Jenkins Successful Pipeline
- Maven Build Success
- Docker Image Build
- Docker Hub Repository
- AWS EC2 Instance
- AWS S3 Bucket
- Kubernetes Nodes
- Kubernetes Running Pods
- Kubernetes Deployment

Example:

markdown
![Kubernetes Pods](screenshots/pods.png)


## 🎯 Key Learning Outcomes

- Linux Administration
- Git & GitHub
- Jenkins CI/CD Pipeline
- Maven Build Automation
- Docker Containerization
- Docker Hub Image Management
- AWS EC2 & S3
- Kubernetes Deployment
- Pod Management
- End-to-End DevOps Workflow

## 🚀 Future Enhancements

- Kubernetes Load Balancer
- Application Monitoring
- Centralized Logging
- Automated Rollback
- Kubernetes Health Checks
- CI/CD Notifications

## 👨‍💻 Author

*Bhavesh Patil*

Aspiring AWS Cloud Engineer | DevOps Engineer

---

⭐ If you find this project useful, don't forget to star the repository!
