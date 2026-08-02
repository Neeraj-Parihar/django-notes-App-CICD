# Django Notes App with Docker & CI/CD

A simple **Notes Application** built using **Django** for the backend and **React** for the frontend. This project demonstrates containerization with **Docker** and is suitable for learning deployment and CI/CD workflows.

---

## Features

* Create, update, and delete notes
* React frontend
* Django REST backend
* Dockerized application
* Ready for CI/CD integration
* Nginx support for reverse proxy

---

## Tech Stack

* Python 3.9+
* Django
* React
* Docker
* Docker Compose
* Nginx

---

## Prerequisites

Make sure the following are installed on your system:

* Python 3.9 or later
* Node.js
* Docker
* Docker Compose
* Git

---

## Clone the Repository

```bash
git clone https://github.com/Neeraj-Parihar/django-notes-App-CICD.git
cd django-notes-App-CICD
```

---

## Build the Docker Image

```bash
docker build -t django-notes-app .
```

---

## Run the Application

```bash
docker run -d -p 8000:8000 django-notes-app
```

The application will be available at:

```
http://localhost:8000
```

---

## Using Docker Compose

Start all services:

```bash
docker compose up --build
```

Run in detached mode:

```bash
docker compose up -d
```

Stop the services:

```bash
docker compose down
```

---

## Nginx Reverse Proxy

Install Nginx:

```bash
sudo apt update
sudo apt install nginx
```

Configure Nginx as a reverse proxy to expose the Django application on ports 80 or 443.

---

## Project Structure

```
django-notes-App-CICD/
├── backend/
├── frontend/
├── docker-compose.yml
├── Dockerfile
├── nginx/
├── requirements.txt
└── README.md
```

---

## Author

**Neeraj Parihar**

GitHub: https://github.com/Neeraj-Parihar
