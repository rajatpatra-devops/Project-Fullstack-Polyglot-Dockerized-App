# 🚀 Fullstack Polyglot Dockerized App

This is a containerized fullstack application built using multiple technologies across different stacks, integrated with **Docker Compose**. The app demonstrates how different languages and services can work together in a microservice-like architecture.

## 🛠️ Tech Stack

- 🌐 **Frontend (React)** – *(commented out for now)*
- 🧠 **Backend (Node.js + Express)**
- 🛢️ **Databases:**
  - MongoDB (NoSQL)
  - PostgreSQL (SQL, for Flask - currently disabled)
- 🐍 **Flask Microservice** – *(commented out for now)*
- 🌐 **Nginx** – acts as reverse proxy to serve the Node.js API
- 🐳 Docker & Docker Compose

## 📁 Project Structure

```bash
fullstack-polyglot-app/
│
├── docker-compose.yml
├── node-backend/          # Node.js + MongoDB app
├── flask-backend/         # Flask app (PostgreSQL) - optional
├── react-frontend/        # React frontend - optional
├── nginx/                 # Custom Nginx config
├── mongo-data/            # MongoDB data volume (not pushed to GitHub)
└── postgres-data/         # PostgreSQL data volume (not pushed to GitHub)

# Clone the repo
git clone https://github.com/rajatpatra-devops/Project-Fullstack-Polyglot-Dockerized-App.git
cd Project-Fullstack-Polyglot-Dockerized-App

# Build & start the containers
docker-compose up --build

⚠️ Known Issues
MongoDB fails on CPUs without AVX support

You can switch to an older version like mongo:4.4 in docker-compose.yml if needed.
