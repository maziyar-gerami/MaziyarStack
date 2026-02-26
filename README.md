# MaziyarStack

**MaziyarStack** is a curated stack of infrastructure and service configurations — a collection of ready‑to‑use deployment and orchestration setups for popular tools and platforms. The goal is to provide a cohesive and opinionated base for building, deploying, and managing various services in a reproducible and consistent environment.

---

## 🧩 Included Components

This repository contains configuration and deployment templates for the following services:

| Service      | Purpose                                           |
|-------------|--------------------------------------------------|
| **Appsmith**  | Open‑source low‑code framework for building internal tools |
| **Nginx**     | Reverse proxy and web server configurations    |
| **Ollama**    | Local model server or AI service integration  |
| **Portainer** | UI for Docker and Kubernetes container management |
| **Swagger**   | API documentation and client generation tooling |
| **WikiJs**    | Modern wiki platform powered by Node.js       |
| **WordPress** | Popular CMS for websites and blogs           |
| **.gitignore**| Common patterns to ignore in version control |

> 💡 Each folder represents infrastructure, deployment, or configuration files related to the named service. You can customize them to suit your environment.

---

## 🚀 Getting Started

> ⚠️ This README assumes familiarity with **Docker**, **Docker Compose**, and typical DevOps workflows. Adjust commands and paths according to your system setup.

### 1. Clone the Repository

```sh
git clone https://github.com/maziyar-gerami/MaziyarStack.git
cd MaziyarStack
```
### 2. Inspect Service Folders

Each directory contains service‑specific configuration:

ls
# Appsmith  Nginx  Ollama  Portainer  Swagger  WikiJs  Wordpress  .gitignore
### 3. Run with Docker Compose (if applicable)

If a folder includes a docker-compose.yml file:
```sh
cd <folder>
docker compose up -d
```
### 4. Access Services

Once deployed:

Nginx — Proxy or gateway (http://localhost)

Appsmith — Internal app platform

Portainer — Container management UI

Swagger UI — API docs viewer

WikiJs — Documentation/wiki interface

WordPress — Website/CMS dashboard

🔧 Note: Service endpoints depend on your network configuration and the port mappings defined in each folder.

🛠 How to Use This Stack

You can use this repository as:

A local development stack

A basis for staging or production deployment

A starting point for custom infrastructure templates

Reference templates for configuration best practices

📦 Prerequisites

Make sure you have the following installed:

Docker Engine (20.x+)

Docker Compose (v2+)

A reverse proxy (e.g., Nginx)

Optional: Traefik, certbot/Let’s Encrypt for SSL termination

📁 Folder Structure & Responsibilities
Directory	Description
Appsmith/	Appsmith deployment & overrides
Nginx/	Nginx configuration, proxy rules, SSL support
Ollama/	AI model server or LLM integrations
Portainer/	Portainer UI and data persistence
Swagger/	API documentation specs and UI configs
WikiJs/	WikiJs service with persistent storage
Wordpress/	WordPress + database configurations
💡 Tips

Use environment variables for sensitive credentials.

Modularize each service for easy reuse with other projects.

Add CI/CD (e.g., GitHub Actions) to automate deployments.

🧪 Testing

To test production‑like flows:

# Example:
docker compose -f Portainer/docker-compose.yml up --build
docker compose -f Wordpress/docker-compose.yml up --build
📄 License

Specify a license for this project (e.g., MIT, Apache‑2.0, etc.) — if you want others to reuse and contribute.

🙌 Contributing

Contributions are welcome!
Feel free to open issues, propose pull requests, or suggest new service folders and templates.
