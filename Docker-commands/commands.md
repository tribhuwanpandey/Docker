commonly used **Docker commands** along with their usage.

---

##  1. Docker System Commands

- **Check Docker version**
  ```bash
  docker --version
  docker version
  ```

- **Check Docker system information**
  ```bash
  docker info
  ```

- **Show all Docker system-wide information (containers, images, volumes, etc.)**
  ```bash
  docker system df
  ```

- **Prune unused objects (containers, networks, images, build cache)**
  ```bash
  docker system prune -a
  ```

---

##  2. Docker Image Commands

- **List all images**
  ```bash
  docker images
  ```

- **Download (pull) an image**
  ```bash
  docker pull <image_name>:<tag>
  ```

- **Build an image from Dockerfile**
  ```bash
  docker build -t <image_name>:<tag> .
  ```

- **Remove an image**
  ```bash
  docker rmi <image_id>
  ```

- **Tag an image**
  ```bash
  docker tag <source_image>:<tag> <target_repo>:<tag>
  ```

- **Push image to registry**
  ```bash
  docker push <repo>/<image_name>:<tag>
  ```

---

##  3. Docker Container Commands

- **List running containers**
  ```bash
  docker ps
  ```

- **List all containers (running + stopped)**
  ```bash
  docker ps -a
  ```

- **Run a container**
  ```bash
  docker run -it --name <container_name> <image_name>
  ```

- **Run a container in detached mode**
  ```bash
  docker run -d <image_name>
  ```

- **Start a stopped container**
  ```bash
  docker start <container_id>
  ```

- **Stop a running container**
  ```bash
  docker stop <container_id>
  ```

- **Restart a container**
  ```bash
  docker restart <container_id>
  ```

- **Pause a container**
  ```bash
  docker pause <container_id>
  ```

- **Unpause a container**
  ```bash
  docker unpause <container_id>
  ```

- **Kill a container**
  ```bash
  docker kill <container_id>
  ```

- **Remove a container**
  ```bash
  docker rm <container_id>
  ```

- **Execute a command inside a running container**
  ```bash
  docker exec -it <container_id> <command>
  ```

- **Attach to a running container**
  ```bash
  docker attach <container_id>
  ```

- **Inspect container details**
  ```bash
  docker inspect <container_id>
  ```

- **View container logs**
  ```bash
  docker logs <container_id>
  ```

- **Copy files from host to container**
  ```bash
  docker cp <host_path> <container_id>:<container_path>
  ```

- **Copy files from container to host**
  ```bash
  docker cp <container_id>:<container_path> <host_path>
  ```

---

##  4. Docker Network Commands

- **List networks**
  ```bash
  docker network ls
  ```

- **Create a network**
  ```bash
  docker network create <network_name>
  ```

- **Inspect a network**
  ```bash
  docker network inspect <network_name>
  ```

- **Connect a container to a network**
  ```bash
  docker network connect <network_name> <container_id>
  ```

- **Disconnect a container from a network**
  ```bash
  docker network disconnect <network_name> <container_id>
  ```

- **Remove a network**
  ```bash
  docker network rm <network_name>
  ```

---

##  5. Docker Volume Commands

- **List volumes**
  ```bash
  docker volume ls
  ```

- **Create a volume**
  ```bash
  docker volume create <volume_name>
  ```

- **Inspect a volume**
  ```bash
  docker volume inspect <volume_name>
  ```

- **Remove a volume**
  ```bash
  docker volume rm <volume_name>
  ```

- **Prune unused volumes**
  ```bash
  docker volume prune
  ```

---

##  6. Docker Compose Commands

- **Start services in background**
  ```bash
  docker-compose up -d
  ```

- **Start services in foreground**
  ```bash
  docker-compose up
  ```

- **Stop services**
  ```bash
  docker-compose down
  ```

- **Build images**
  ```bash
  docker-compose build
  ```

- **Restart services**
  ```bash
  docker-compose restart
  ```

- **View logs**
  ```bash
  docker-compose logs
  ```

---

##  7. Useful Docker Tips

- **Remove all stopped containers**
  ```bash
  docker container prune
  ```

- **Remove all unused images**
  ```bash
  docker image prune -a
  ```

- **Remove all unused networks**
  ```bash
  docker network prune
  ```

- **Remove everything (containers, images, networks, volumes)**
  ```bash
  docker system prune -a --volumes
  ```

---
