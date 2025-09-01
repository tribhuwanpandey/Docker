#  Docker Flask + Redis + Nginx Project

This project demonstrates a simple **multi-container application** using:

- **Flask (Python)** — web app
- **Redis** — counter backend
- **Nginx** — reverse proxy
- **Docker Compose** — orchestration

---

##  Features

- View count stored and retrieved from Redis
- Flask handles HTTP requests
- Nginx proxies traffic to Flask app
- Fully containerized stack using Docker Compose

---

##  Project Structure

docker-flask-redis/
│
├── app/
│   ├── app.py
│   ├── requirements.txt
│   └── Dockerfile
│
├── nginx/
│   └── default.conf
│
├── docker-compose.yml
└── README.md



## Description

- **`app/`**: Contains the Flask application code.
- **`nginx/`**: Holds the Nginx configuration used to reverse proxy requests to the Flask app.
- **`docker-compose.yml`**: Defines and runs multi-container Docker applications.
- **`README.md`**: Documentation for understanding the project structure and setup.
