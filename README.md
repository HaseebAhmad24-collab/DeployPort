# 🚢 DeployPort

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](#)
[![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)](#)
[![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)](#)
[![Jenkins](https://img.shields.io/badge/jenkins-%23D24939.svg?style=for-the-badge&logo=jenkins&logoColor=white)](#)

**DeployPort** is a streamlined, production-ready containerized deployment template for personal portfolios and static websites. By combining the performance of Nginx with the portability of Docker and the automation of Jenkins, this project provides a "DevOps-first" foundation for showcasing professional work.

---

## ✨ Features

-   **⚡ Ultra-Lightweight:** Built on Nginx Alpine, ensuring a minimal resource footprint and fast container startup times.
-   **🐳 Containerized Workflow:** Complete environment parity from development to production using Docker.
-   **🔄 Automated CI/CD:** Pre-configured `Jenkinsfile` to automate the build and deployment lifecycle.
-   **🌐 Production Grade:** Optimized Nginx configuration for serving static assets efficiently.
-   **📱 Fully Responsive:** The core HTML structure is designed to be accessible across all device types.

---

## 🛠️ Tech Stack

-   **Frontend:** HTML5
-   **Web Server:** Nginx (Alpine Linux)
-   **Orchestration:** Docker
-   **Automation:** Jenkins Pipeline (Groovy)

---

## 🚀 Getting Started

### Prerequisites

-   [Docker](https://www.docker.com/get-started) installed on your local machine.
-   [Git](https://git-scm.com/) for version control.

### Installation & Local Setup

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/HaseebAhmad24-collab/DeployPort.git
    cd DeployPort
    ```

2.  **Build the Docker Image**
    ```bash
    docker build -t deployport-site .
    ```

3.  **Run the Container**
    ```bash
    docker run -d -p 8080:80 --name my-portfolio deployport-site
    ```

4.  **Verify Deployment**
    Navigate to `http://localhost:8080` in your preferred web browser.

---

## 🏗️ CI/CD Pipeline

This project includes a `Jenkinsfile` designed to handle the continuous integration process. The pipeline typically follows these stages:

1.  **Checkout:** Pulls the latest source code from the main branch.
2.  **Build:** Packages the HTML assets into a new Docker image.
3.  **Test:** (Optional) Validates the Nginx configuration.
4.  **Deploy:** Pushes the finalized image to your container registry or updates the running service.

---

## 📂 Project Structure

```text
DeployPort/
├── Dockerfile          # Nginx Alpine container configuration
├── Jenkinsfile         # CI/CD pipeline automation script
├── README.md           # Project documentation
└── index.html          # Main website entry point
```

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## ⚖️ License

Distributed under the MIT License. See `LICENSE` for more information.

---

**Maintained by [Haseeb Ahmad](https://github.com/HaseebAhmad24-collab)**