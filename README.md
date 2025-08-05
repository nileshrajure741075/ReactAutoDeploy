# ReactAutoDeploy


# 🚀 CI/CD Pipeline for React App Deployment on AWS EC2 with Jenkins

This project demonstrates a complete CI/CD pipeline using Jenkins to automate the deployment of a React application from GitHub to an AWS EC2 instance using Docker.

## 🔧 Technologies Used

- React.js (Frontend)
- Jenkins (CI/CD Pipeline)
- Docker (Containerization)
- AWS EC2 (Deployment Target)
- GitHub (Source Code Repository)
- Nginx (Serving the Build)

## 📂 Project Structure

```
.
├── Dockerfile
├── docker-compose.yml
├── Jenkinsfile
├── package.json
├── README.md
└── src/
```

## ⚙️ Jenkins Pipeline Stages

1. **Clone Code** – Clones React app from GitHub repository.
2. **Build Image** – Builds Docker image using a multi-stage Dockerfile.
3. **Test** – Optional placeholder for automated tests.
4. **Deploy** – Runs the image as a container using Docker.

## 🐳 Docker Commands

To build and run the container manually:
```bash
docker build -t react-app .
docker run -d -p 80:80 react-app
```

## 🖥️ EC2 Setup

- Ubuntu EC2 instance with Docker and Jenkins installed.
- Jenkins agent (labeled `vinod`) used to run the pipeline.
- Port 80 opened in the EC2 security group to access the app.

## 🧪 Webhook Integration

- Configured GitHub webhook to trigger Jenkins pipeline on every push.

## 📷 Demo Screenshot

*(Insert image if available)*

## 📜 License

This project is for educational and demo purposes.
