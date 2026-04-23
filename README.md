# Portfolio Website

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Jenkins](https://img.shields.io/badge/jenkins-%23D24939.svg?style=for-the-badge&logo=jenkins&logoColor=white)

A high-performance, containerized personal portfolio website. This project showcases a professional profile using a streamlined tech stack optimized for speed, portability, and automated deployment.

## 🚀 Overview

This repository contains the source code for a responsive portfolio site. Unlike traditional static hosting, this project is built with a **DevOps-first approach**, utilizing Docker for environment parity and Jenkins for continuous integration and delivery (CI/CD).

## ✨ Features

- **Lightweight Core:** Built with clean, semantic HTML5.
- **Containerized Architecture:** Powered by Nginx on Alpine Linux for an ultra-small footprint.
- **CI/CD Ready:** Includes a `Jenkinsfile` for automated build and deployment pipelines.
- **Production-Grade Web Server:** Uses Nginx to serve content efficiently.
- **Responsive Design:** Optimized for viewing across all device types.

## 🛠️ Installation & Setup

You can run this portfolio locally either by opening the files directly or using Docker for a production-like environment.

### Option 1: Using Docker (Recommended)

1. **Clone the repository:**
   ```bash
   git clone https://github.com/HaseebAhmad24-collab/portfolio.git
   cd portfolio
   ```

2. **Build the Docker image:**
   ```bash
   docker build -t my-portfolio .
   ```

3. **Run the container:**
   ```bash
   docker run -d -p 8080:80 --name portfolio-site my-portfolio
   ```

4. **Access the site:**
   Open your browser and navigate to `http://localhost:8080`.

### Option 2: Manual Execution

Simply open the `index.html` file in any modern web browser.

## 🔄 CI/CD Pipeline

The project includes a `Jenkinsfile` which automates the following workflow:
1. **Source:** Pulls the latest code from the repository.
2. **Build:** Creates a Docker image based on the provided `Dockerfile`.
3. **Deploy:** (Configurable) Pushes the image to a registry or deploys to a web server.

## 📂 Project Structure

```text
.
├── Dockerfile          # Multi-stage build configuration
├── Jenkinsfile         # CI/CD pipeline definition
└── index.html          # Main portfolio entry point
```

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the design or add features:

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## ⚖️ License

Distributed under the MIT License. See `LICENSE` for more information.

---
**Maintained by [Haseeb Ahmad](https://github.com/HaseebAhmad24-collab)**