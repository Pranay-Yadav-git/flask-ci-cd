# Flask App CI/CD with GitHub Actions

This project demonstrates a dynamic web application using Flask, Docker, and CI/CD via GitHub Actions.

## Features
- Python Flask app
- Dockerized for portability
- GitHub Actions to automate build & push to Docker Hub

## How to Run Locally
```bash
docker build -t flask-app .
docker run -p 5000:5000 flask-app
```

## Deployment via GitHub Actions
Push to `main` branch triggers workflow:
1. Builds Docker image
2. Pushes image to Docker Hub

Make sure to set secrets in GitHub:
- `DOCKER_USERNAME`
- `DOCKER_PASSWORD`
