# Node.js Demo App with CI/CD 🚀

This is a simple Node.js + Express web application that includes:
- A full CI/CD pipeline using **GitHub Actions**
- Docker image build and push to **DockerHub**
- Automatic **deployment to a remote server via SSH**
- A styled HTML frontend with a **background image**

## 🌐 Live Features

- **Homepage** (`/`) with background image and heading
- **Health Check** (`/health`) returns app uptime as JSON

## 🛠 Technologies Used

- Node.js & Express
- HTML/CSS frontend
- Docker & DockerHub
- GitHub Actions CI/CD
- Remote deployment via SSH

## 🔐 GitHub Secrets Required

| Secret Name      | Description                                |
|------------------|--------------------------------------------|
| `DOCKER_USERNAME`| Your DockerHub username                    |
| `DOCKER_PASSWORD`| DockerHub password or access token         |
| `SERVER_IP`      | Public IP of your server (e.g., EC2)       |
| `SSH_USERNAME`   | SSH username (e.g., `ubuntu`, `ec2-user`)  |
| `SSH_KEY`        | Base64-encoded private SSH key             |

To encode your key:
```bash
base64 ~/.ssh/id_rsa
