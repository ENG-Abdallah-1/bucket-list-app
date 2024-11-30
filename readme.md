
# Flask Bucket List App




## Overview
This project is a Flask-based web application that allows users to manage their personal goals and tasks. It includes features like user authentication, session management, and CRUD operations for "wishes." The app is built for scalability and includes deployment-ready configurations.

## Features
- User authentication (Sign Up/Sign In)
- Session management
- CRUD operations for managing "wishes"
- MySQL database integration
- Dockerized setup for easy deployment
- CI/CD pipelines using Jenkins
- Kubernetes manifests for container orchestration
- Infrastructure as Code (IaC) using Terraform
- Automation with Ansible playbooks

## About the Project
This project is part of my graduation in the **DEPI - Digital Egypt Pioneers Initiative**, under the **DevOps track**. It showcases end-to-end application deployment, automation, and infrastructure management.

## Project Structure
```
- ansible_playbooks/         # Ansible scripts for automation
- k8s_manifests/             # Kubernetes YAML manifests for deployment
- Sprints_WS_final/          # Final sprint workspace and related files
- terraform_scripts/         # Terraform files for infrastructure provisioning
- app.py                     # Flask application logic
- templates/                 # HTML templates for the app's frontend
- static/                    # Static assets like CSS and JavaScript
- Dockerfile                 # Docker configuration
- docker-compose.yml         # Multi-container setup
- *.sql                      # Database scripts
```

## Prerequisites
- Python 3.8+
- Docker
- Kubernetes
- MySQL
- Terraform
- Jenkins

## Setup and Deployment
1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Set Up Environment Variables**
   Create a `.env` file with the following variables:
   ```
   MYSQL_DATABASE_USER=your_username
   MYSQL_DATABASE_PASSWORD=your_password
   MYSQL_DATABASE_DB=your_database_name
   MYSQL_DATABASE_HOST=your_database_host
   ```

3. **Build and Run with Docker**
   ```bash
   docker-compose up --build
   ```

4. **Deploy to Kubernetes**
   Apply the Kubernetes manifests:
   ```bash
   kubectl apply -f k8s_manifests/
   ```

5. **Provision Infrastructure with Terraform**
   ```bash
   terraform init
   terraform apply
   ```

## Usage
- Visit the homepage to sign up or sign in.
- Add, view, update, or delete your personal goals.



## Contributing
Feel free to fork the repository and submit pull requests for improvements or bug fixes.
