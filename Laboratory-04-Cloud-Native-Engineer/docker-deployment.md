# Docker Deployment

**Student Name:** Jhuniel Laureta
**Subject:** CCM101 – Cloud Computing
**Laboratory:** Laboratory 04 – Cloud-Native Engineer

## 1. Docker Environment Verification

Before deploying the containerized web server, I verified that Docker was installed and running in the KillerCoda Linux environment.

### Check Docker Version

```bash
docker --version
```

This command was used to check the installed version of Docker in the Linux environment.

### Check Docker Environment

```bash
docker info
```

This command was used to check the current Docker environment and confirm that the Docker engine was available.

## 2. Deploy Nginx Container

### Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image so it can be used to create a container.

### Run the Nginx Container

```bash
docker run -d -p 8080:80 --name nginx-server nginx
```

This command creates and starts an Nginx container in detached mode. The `-p 8080:80` option maps port 8080 of the host to port 80 inside the Nginx container, while `--name nginx-server` gives the container a specific name.

### Test the Nginx Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx web server through port 8080 and verifies that the containerized web server is running successfully.

The successful result displayed the HTML content of the Nginx welcome page, including the message:

```text
Welcome to nginx!
```

## 3. Container Lifecycle

### 3.1 List Running Containers

```bash
docker ps
```

This command displays the containers that are currently running, including the `nginx-server` container.

### 3.2 Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running `nginx-server` container.

### 3.3 Verify That the Container Is Stopped

```bash
docker ps
```

This command checks the currently running containers and confirms that the stopped `nginx-server` container is no longer running.

### 3.4 View All Containers

```bash
docker ps -a
```

This command displays all Docker containers, including containers that are currently stopped.

### 3.5 Remove the Container

```bash
docker rm nginx-server
```

This command permanently removes the stopped `nginx-server` container from the Docker environment.

### 3.6 Verify the Container Removal

```bash
docker ps -a
```

This command verifies that the `nginx-server` container has been removed and is no longer listed among the containers.

## 4. Complete Docker Command List

The following commands were used during the Docker deployment and container lifecycle activities:

```bash
docker --version
docker info
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080
docker ps
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a
```

## 5. Screenshots

The following screenshots were collected as evidence of the completed Docker activities:

* `docker-version.png` – Shows the Docker version and Docker environment verification.
* `nginx-running.png` – Shows the successful Nginx web server response.
* `container-lifecycle.png` – Shows the Docker container lifecycle commands and their results.

