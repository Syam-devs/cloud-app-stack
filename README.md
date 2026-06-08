# Cloud App Stack

A containerized web application deployed using Docker and Nginx on AWS EC2. This project demonstrates modern DevOps deployment practices, including containerization, cloud hosting, GitHub version control, and infrastructure management.

## Project Overview

Cloud App Stack is a lightweight web platform designed to showcase a production-style deployment workflow. The application is packaged into a Docker container, served through Nginx, and deployed on an AWS EC2 instance.

## Architecture

User Browser
↓
AWS EC2
↓
Docker Container
↓
Nginx Web Server
↓
Static Web Application

## Technologies Used

* AWS EC2
* Docker
* Nginx
* HTML5
* CSS3
* Git
* GitHub
* SSH Authentication

## Features

* Containerized deployment
* Cloud-hosted application
* Nginx web server integration
* Version-controlled source code
* Secure GitHub SSH authentication
* Responsive landing page

## Project Structure

```text
cloud-app-stack/
│
├── index.html
├── style.css
├── Dockerfile
├── docker-compose.yml
└── README.md
```

## Dockerfile

The application uses an Nginx base image and copies static assets into the Nginx web root for serving.

## Deployment Steps

### Clone Repository

```bash
git clone git@github.com:Syam-devs/cloud-app-stack.git
cd cloud-app-stack
```

### Build Docker Image

```bash
docker build -t cloud-app-stack:v1 .
```

### Run Container

```bash
docker run -d -p 80:80 --name cloud-app-stack cloud-app-stack:v1
```

### Verify Deployment

```bash
docker ps
```

### Access Application

Open:

```text
http://<EC2-PUBLIC-IP>
```

## Key Learnings

* Docker image creation
* Container lifecycle management
* Nginx web hosting
* AWS EC2 deployment
* GitHub SSH authentication
* Troubleshooting Docker build issues
* Understanding RUN vs CMD in Dockerfiles

## Future Improvements

* GitHub Actions CI/CD
* Docker Compose multi-service deployment
* HTTPS with SSL certificates
* Infrastructure as Code using Terraform
* Kubernetes deployment
* Monitoring with Prometheus and Grafana

