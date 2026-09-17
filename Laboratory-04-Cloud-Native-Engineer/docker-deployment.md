
# Docker Deployment

## Mission 4: The Cloud-Native Engineer

This document records the Docker commands used to deploy and manage an Nginx web server in the KillerCoda Docker playground.

## 1. Verify Docker Installation

### Command

```bash
docker --version
```

This command displays the installed Docker version and confirms that Docker is available in the terminal.

### Command

```bash
docker info
```

This command displays information about the Docker environment and helps verify that the Docker daemon is operational.

---

## 2. Pull the Nginx Image

### Command

```bash
docker pull nginx
```

This command downloads the Nginx image so that it can be used to create a container.

---

## 3. Run the Nginx Container

### Command

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command creates and starts an Nginx container in detached mode and maps host port 8080 to port 80 inside the container.

The options mean:

* `-d` — runs the container in the background.
* `--name nginx-server` — gives the container the name `nginx-server`.
* `-p 8080:80` — maps host port 8080 to container port 80.
* `nginx` — specifies the Nginx image to use.

---

## 4. List Running Containers

### Command

```bash
docker ps
```

This command lists the Docker containers that are currently running.

The Nginx container should appear in the list with port `8080` mapped to container port `80`.

---

## 5. Test the Nginx Web Server

### Command

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx web server through port 8080 and displays the server's response in the terminal.

A successful response should contain the Nginx welcome page HTML.

---

## 6. Stop the Running Container

### Command

```bash
docker stop nginx-server
```

This command stops the running Nginx container while keeping the container available on the system.

---

## 7. Verify That the Container Is Stopped

### Command

```bash
docker ps
```

This command displays only running containers, so the stopped Nginx container should no longer appear.

To display both running and stopped containers, use:

```bash
docker ps -a
```

This confirms that the Nginx container still exists but has stopped running.

---

## 8. Remove the Container

### Command

```bash
docker rm nginx-server
```

This command removes the stopped Nginx container from the Docker environment.

The container must normally be stopped before it can be removed with this command.

---

## 9. Verify That the Container Was Removed

### Command

```bash
docker ps -a
```

This command lists all containers and can be used to confirm that `nginx-server` has been removed.

---

## Container Lifecycle Summary

The main container lifecycle commands used in this activity were:

```bash
docker ps
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a
```

The activity demonstrated the basic lifecycle of a Docker container: **create/run → inspect → stop → remove**.

## Screenshots

The following screenshots provide evidence of the Docker deployment and container lifecycle:

* `screenshots/docker-version.png` — Docker installation and environment verification.
